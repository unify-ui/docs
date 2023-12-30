<script setup lang="ts">
import ShowCaseBasicUsage from './ShowCaseBasicUsage.vue';
import ShowCasePlaceholder from './ShowCasePlaceholder.vue';
import ShowCaseDisabled from './ShowCaseDisabled.vue';
</script>

# Password

## Basic usage

::: raw
<ClientOnly>
<ShowCaseBasicUsage class="vp-raw" />
</ClientOnly>
:::

::: details View Source
<<< @/components/data-entry/password/ShowCaseBasicUsage.vue
:::

## Placeholder

::: raw
<ClientOnly>
<ShowCasePlaceholder class="vp-raw" />
</ClientOnly>
:::

::: details View Source
<<< @/components/data-entry/password/ShowCasePlaceholder.vue
:::

## Disabled

::: raw
<ClientOnly>
<ShowCaseDisabled class="vp-raw" />
</ClientOnly>
:::

::: details View Source
<<< @/components/data-entry/password/ShowCaseDisabled.vue
:::

## API

### Properties

```ts
const props = withDefaults(
  defineProps<{
    modelValue?: string;
    disabled?: boolean;
    placeholder?: string;
  }>(),
  {
    modelValue: "",
    placeholder: "",
  }
);
```

### Events

```ts
defineEmits<{
  (e: "update:modelValue", value: string): void;
  (e: "input", value: string): void;
  (e: "change", value: string): void;
}>();
```
