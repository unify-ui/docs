<script setup lang='ts'>
import ShowCaseBasicUsage from './ShowCaseBasicUsage.vue'
import ShowCaseDisabled from './ShowCaseDisabled.vue'
</script>

# Tooltip

## Basic Usage

::: raw
<ClientOnly>
<ShowCaseBasicUsage class="vp-raw" />
</ClientOnly>
:::

::: details View Source
<<< @/components/data-display/tooltip/ShowCaseBasicUsage.vue
:::

## Disabled

::: raw
<ClientOnly>
<ShowCaseDisabled class="vp-raw" />
</ClientOnly>
:::

::: details View Source
<<< @/components/data-display/tooltip/ShowCaseDisabled.vue
:::

## API

### Properties

```ts
withDefaults(
  defineProps<{
    /** The content of the tooltip */
    title: string;
    /** The placement of the tooltip */
    placement: "top" | "bottom" | "left" | "right";
    /** Whether the tooltip is disabled */
    disabled?: boolean;
    /** Append */
    appendToBody?: boolean;
  }>(),
  {
    appendToBody: true,
  }
);
```
