<script setup lang='ts'>
import ShowCaseBasicUsage from './ShowCaseBasicUsage.vue'
import ShowCaseDisabled from './ShowCaseDisabled.vue'
import ShowCaseNoLabel from './ShowCaseNoLabel.vue' 
import ShowCaseIndeterminate from './ShowCaseIndeterminate.vue'
</script>

# Checkbox

## Basic Usage

::: raw
<ClientOnly>
<ShowCaseBasicUsage class="vp-raw" />
</ClientOnly>
:::

::: details View Source
<<< @/components/data-entry/checkbox/ShowCaseBasicUsage.vue
:::

## Disabled

::: raw
<ClientOnly>
<ShowCaseDisabled class="vp-raw" />
</ClientOnly>
:::

::: details View Source
<<< @/components/data-entry/checkbox/ShowCaseDisabled.vue
:::

## No Label

::: raw
<ClientOnly>
<ShowCaseNoLabel class="vp-raw" />
</ClientOnly>
:::

::: details View Source
<<< @/components/data-entry/checkbox/ShowCaseNoLabel.vue
:::

## Indeterminate

::: raw
<ClientOnly>
<ShowCaseIndeterminate class="vp-raw" />
</ClientOnly>
:::

::: details View Source
<<< @/components/data-entry/checkbox/ShowCaseIndeterminate.vue
:::

## API

### Properties

```ts
const props = withDefaults(
  defineProps<{
    label?: string;
    checked?: boolean;
    value?: Value;
    disabled?: boolean;
    indeterminate?: boolean;
  }>(),
  {
    label: "",
    value: void 0,
    disabled: false,
  }
);
```

### Events

```ts
const emit = defineEmits<{
  (e: "update:checked", checked: boolean): void;
  (e: "change", checked: boolean): void;
}>();
```
