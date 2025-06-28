### Replication steps :-

- Create a new Vue app using npm create vue@latest
- Choose Rolldown build option
- Import [VueDraggable](https://github.com/SortableJS/vue.draggable.next) in any component. Note you need the `next` branch for Vue 3.
- Create a build and preview it locally [vite build, vite preview]

Uncaught TypeError: F is not a function this error gets thrown and the application breaks.

## Notes :-

- `import Draggable from 'vuedraggable'` breaks Rolldown build
- Works properly on a local dev server and with Rollup build.
- Might be a compat issue, switching the import to `import Draggable from 'vuedraggable/src/vuedraggable'` works.
