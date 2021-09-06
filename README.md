# Hello-vue
The most useable vue code on project!

### Vue looping.
```
<some-component v-for="(row, id) in filter" :key="id" :data="[array]" />
```
### Simple toogle statement
```
<buton @click="open = !open">open now!</button>


<div v-if="open">hello</div>
or
<div v-show="open">hello</div>

data(){ return : { open = false }}

```

### Big scale vue-router
Vue Router structure data for big scale project.
