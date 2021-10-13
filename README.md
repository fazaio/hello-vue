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

### Editable Table data inside v-for loop
Using $ref to select DOM element
```
<input
v-on:keyup.enter="do_edit_warehouse_loc(id, row)"
:ref="`warehouse_loc${id}`"
@click="edit_warehouse_loc(id)"
@blur="edit = false"
v-bind:class="{ edit : id == edit }"
class="p-2 m-0 text-right outline-none rounded"
type="text"
:value="row.SPShipping.warehouse_loc"
readonly/>
```


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
