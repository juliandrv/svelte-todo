<script lang="ts">
  type CompletedTodosType = number;
  type ClearCompletedType = () => void;

  export let completedTodos: CompletedTodosType;
  export let clearCompleted: ClearCompletedType;
</script>

<button
  on:click={clearCompleted}
  class:hidden={completedTodos === 0}
  class="clear-completed"
>
  {completedTodos} completed
</button>
