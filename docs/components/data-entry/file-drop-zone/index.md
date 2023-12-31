<script setup lang='ts'>
import ShowCaseBasicUsage from './ShowCaseBasicUsage.vue'
import ShowCaseMultipleFiles from './ShowCaseMultipleFiles.vue'
import ShowCasePromptText from './ShowCasePromptText.vue'
import ShowCaseCustomizedContent from './ShowCaseCustomizedContent.vue'
</script>

# FileDropZone

## Basic Usage

::: raw
<ShowCaseBasicUsage />
:::

::: details View Source
<<< @/components/data-entry/file-drop-zone/ShowCaseBasicUsage.vue
:::

## Multiple Files

::: raw
<ShowCaseMultipleFiles />
:::

::: details View Source
<<< @/components/data-entry/file-drop-zone/ShowCaseMultipleFiles.vue
:::

## Customized Prompt Text

::: raw
<ShowCasePromptText />
:::

::: details View Source
<<< @/components/data-entry/file-drop-zone/ShowCasePromptText.vue
:::

## Customized Content

::: raw
<ShowCaseCustomizedContent />
:::

::: details View Source
<<< @/components/data-entry/file-drop-zone/ShowCaseCustomizedContent.vue
:::

## API

### Properties

```ts
const props = defineProps<{
  promptText?: string;
  multiple?: boolean;
}>();
```

### Events

```ts
const emits = defineEmits<{
  (e: "file-change", files: File[]): void;
}>();
```

### Slots

```ts
defineSlots<{
  default?: (props: {}) => any;
}>();
```
