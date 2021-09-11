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


### Computed filter object of array
```
    filter() {
      var data = this.data;
      const allowed = this.find;
      if ("" !== allowed) {
        return data.filter((e) => e.title.includes(allowed));
      }
      return data;
    },
```
