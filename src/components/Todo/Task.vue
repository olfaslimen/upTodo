<template>
  <div>
    <v-list-item
      @click="$store.commit('doneTask', task.id)"
      :class="{ 'red lighten-5' : task.done }"
      :ripple="false"
    >
      <template v-slot:default>
        <v-list-item-action>
          <v-checkbox
            :input-value="task.done"
            color="#E57373"   
            ></v-checkbox>
        </v-list-item-action>

        <v-list-item-content>
          <v-list-item-title
            :class="{ 'text-decoration-line-through' : task.done }"
          >
            {{ task.title }}
          </v-list-item-title>
        </v-list-item-content>

        <v-list-item-action v-if="task.dueDate">
          <v-list-item-action-text color="#E57373">
            <v-icon small color="#E57373">mdi-calendar</v-icon>
            {{ task.dueDate | niceDate }}
          </v-list-item-action-text>
        </v-list-item-action>

        <v-list-item-action>
          <task-menu :task="task" />
        </v-list-item-action>
        <!-- sort buttom   -->
        <v-list-item-action
        v-if="$store.state.sorting"
        >
          <v-btn
          color="#E57373"
          icon
          class="handle"
          >
          <v-icon>mdi-drag-horizontal-variant</v-icon>
          </v-btn>
        </v-list-item-action>
      </template>

    </v-list-item>
    <v-divider></v-divider>

  </div>
</template>

<script>
import { format } from 'date-fns'


export default {
  props: ['task'],
  filters: {
    niceDate(value) {
      return format(new Date(value), 'MMM d')
    }
  },
  components: {
    'task-menu': require('@/components/Todo/TaskMenu.vue').default,
  }
}
</script>