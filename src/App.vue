<template>
  <div id="root">
    <div class="todoapp">
      <h1 class="todoapp__title">todos</h1>
      <div class="todoapp__content">
        <header class="todoapp__header">
          <button
            type="button"
            class="todoapp__toggle-all"
            data-cy="ToggleAllButton"
          ></button>
          <form>
            <input
              data-cy="NewTodoField"
              type="text"
              class="todoapp__new-todo"
              placeholder="What needs to be done?"
              value=""
            />
          </form>
        </header>
        <section class="todoapp__main" data-cy="TodoList">
          <div>
            <div data-cy="Todo" class="todo">
              <label class="todo__status-label" for="todo-status-276557"
                ><input
                  id="todo-status-276557"
                  data-cy="TodoStatus"
                  type="checkbox"
                  class="todo__status" /></label
              ><span data-cy="TodoTitle" class="todo__title">dasda</span
              ><button type="button" class="todo__remove" data-cy="TodoDelete">
                ×
              </button>
              <div data-cy="TodoLoader" class="modal overlay">
                <div class="modal-background has-background-white-ter"></div>
                <div class="loader"></div>
              </div>
            </div>
            <div data-cy="Todo" class="todo">
              <label class="todo__status-label" for="todo-status-276558"
                ><input
                  id="todo-status-276558"
                  data-cy="TodoStatus"
                  type="checkbox"
                  class="todo__status" /></label
              ><span data-cy="TodoTitle" class="todo__title">dasdadasda</span
              ><button type="button" class="todo__remove" data-cy="TodoDelete">
                ×
              </button>
              <div data-cy="TodoLoader" class="modal overlay">
                <div class="modal-background has-background-white-ter"></div>
                <div class="loader"></div>
              </div>
            </div>
          </div>
        </section>
        <footer class="todoapp__footer" data-cy="Footer">
          <span class="todo-count" data-cy="TodosCounter">2 items left</span>
          <nav class="filter" data-cy="Filter">
            <a href="#/" class="filter__link selected" data-cy="FilterLinkAll"
              >All</a
            ><a href="#/active" class="filter__link" data-cy="FilterLinkActive"
              >Active</a
            ><a
              href="#/completed"
              class="filter__link"
              data-cy="FilterLinkCompleted"
              >Completed</a
            >
          </nav>
          <button
            type="button"
            class="todoapp__clear-completed"
            data-cy="ClearCompletedButton"
            disabled=""
          >
            Clear completed
          </button>
        </footer>
      </div>
      <div
        data-cy="ErrorNotification"
        class="notification is-danger is-light has-text-weight-normal hidden"
      >
        <button data-cy="HideErrorButton" type="button" class="delete"></button>
      </div>
    </div>
  </div>
  <!-- <script type="module" src="/src/index.tsx"></script> -->
</template>
