<template>
  <div>
    <h1 class="title-case">{{ resource.title ? resource.title : "Untitled"}}</h1>
    <tag-list :tags="resource.tags" :grid="true" />
  </div>
</template>

<script>
import TagList from "./TagList";

export default {
  components: { TagList },
  props: ["resource"],
};
</script>