<script setup lang='ts'>
import ShowCasePrimaryButton from './ShowCasePrimaryButton.vue'
import ShowCaseSecondaryButton from './ShowCaseSecondaryButton.vue'
import ShowCaseSoftButton from './ShowCaseSoftButton.vue'
import ShowCaseRounded from './ShowCaseRounded.vue'
import ShowCaseDisabled from './ShowCaseDisabled.vue'
</script>

# Button

Unify UI provide 3 types of button.

- Primary Button
- Secondary Button
- Soft Button

## Primary Button

::: raw
<ClientOnly>
<ShowCasePrimaryButton class="vp-raw" />
</ClientOnly>
:::

::: details View Source
<<< @/components/general/button/ShowCasePrimaryButton.vue
:::

## Secondary Button

::: raw
<ClientOnly>
<ShowCaseSecondaryButton class="vp-raw" />
</ClientOnly>
:::

::: details View Source
<<< @/components/general/button/ShowCaseSecondaryButton.vue
:::

## Soft Button

::: raw
<ClientOnly>
<ShowCaseSoftButton class="vp-raw" />
</ClientOnly>
:::

::: details View Source
<<< @/components/general/button/ShowCaseSoftButton.vue
:::

## Rounded Button

::: raw
<ClientOnly>
<ShowCaseRounded class="vp-raw" />
</ClientOnly>
:::

::: details View Source
<<< @/components/general/button/ShowCaseRounded.vue
:::

## Disabled

::: raw
<ClientOnly>
<ShowCaseDisabled class="vp-raw" />
</ClientOnly>
:::

::: details View Source
<<< @/components/general/button/ShowCaseDisabled.vue
:::

## API

### Properties

```ts
withDefaults(
  defineProps<{
    type?: "secondary" | "primary" | "soft";
    size?: "xs" | "s" | "m" | "l" | "xl";
    rounded?: boolean;
    disabled?: boolean;
  }>(),
  {
    type: "secondary",
    size: "m",
  }
);
```

### Events

```ts
const emits = defineEmits<{
  (e: "click", event: MouseEvent): void;
}>();
```

### Slots

```ts
const slots = defineSlots<{
  default(props: {}): any;
}>();
```
