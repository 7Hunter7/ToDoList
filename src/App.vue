<template>
  <div id="app">
    <AppHeader />

    <aside class="app-filters">
      <section class="toggle-group">
        <button class="button button--primary">All</button>
        <button class="button">Active</button>
        <button class="button">Done</button>
      </section>
    </aside>

    <main class="app-main">
      <ul class="todo-list">
        <li class="todo-item todo-item--done">
          <div class="todo-item__status">
            <i class="bi bi-check2"></i>
          </div>
          <span class="todo-item__text">Learn the basics of Vue</span>
          <button class="todo-item__remove-button">
            <i class="bi bi-trash3"></i>
          </button>
        </li>
        <li class="todo-item">
          <div class="todo-item__status">
            <i class="bi bi-check2"></i>
          </div>
          <span class="todo-item__text">Learn the basics of Typescript</span>
          <button class="todo-item__remove-button">
            <i class="bi bi-trash3"></i>
          </button>
        </li>
        <li class="todo-item">
          <div class="todo-item__status">
            <i class="bi bi-check2"></i>
          </div>
          <span class="todo-item__text">Subscribe to the channel</span>
          <button class="todo-item__remove-button">
            <i class="bi bi-trash3"></i>
          </button>
        </li>
      </ul>

      <section class="add-todo">
        <button class="add-todo__show-form-button">
          <i class="bi bi-plus-lg"></i>
        </button>
        <form class="add-todo__form">
          <button class="close-button" type="button">
            <i class="bi bi-x"></i>
          </button>
          <div class="text-input text-input--focus">
            <input class="input" />
          </div>
          <button class="button button--filled">Add task</button>
        </form>
      </section>
    </main>

    <footer class="app-footer">2 more to do, 1 done</footer>
  </div>
</template>

<scriptz lang="ts">
import { defineComponent } from "vue";
import AppHeader from "./components/AppHeader.vue";

export default defineComponent({
  components: {
    AppHeader,
  },
});
</scriptz>
