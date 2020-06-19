<template>
    <div class="mt-3 mt-md-0">
      <div v-for="e in elementsList" v-bind:key="e.id" class="mt-2">
        <router-link :to="'/detail/'+ e.id">
          <b-card :title="e.title">
            <b-card-text>
                {{e.description}}
            </b-card-text>
          </b-card>
        </router-link>
      </div>
    </div>
</template>

<script>
export default {
  props: ["elementsList"],
  data() {
    return {
      elements: []
    };
  },
  methods: {}
};
</script>
