<script lang="ts">
    import { page } from '$app/state';
    import { emojis } from './emojis.js';
</script>

<h1>{page.error?.message ?? 'An error occured'}</h1>

<span style="font-size: 11em">
    {emojis[page.status] ?? emojis[404]}
</span>