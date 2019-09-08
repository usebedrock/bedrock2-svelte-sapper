<script>
    export let icon;

    // Possible icon types
    import IconDelete from './Icons/delete.svg';
    import IconQuestion from './Icons/question.svg';
    import IconAdd from './Icons/add.svg';
    import IconRemove from './Icons/remove.svg';
    import IconMenu from './Icons/menu.svg';
    import IconClose from './Icons/close.svg';
    import IconTime from './Icons/time.svg';
    import IconChevronLeft from './Icons/chevron-left.svg';
    import IconChevronRight from './Icons/chevron-right.svg';

</script>

<style>
    .svg-icon {
        width: 1.6rem;
        height: 1.6rem;
    }

</style>

<div class="svg-icon">
{#if icon == 'delete'}
    {@html IconDelete}
{/if}
{#if icon == 'question'}
    {@html IconQuestion}
{/if}
{#if icon == 'add'}
    {@html IconAdd}
{/if}
{#if icon == 'remove'}
    {@html IconRemove}
{/if}
{#if icon == 'close'}
    {@html IconClose}
{/if}
{#if icon == 'menu'}
    {@html IconMenu}
{/if}
{#if icon == 'time'}
    {@html IconTime}
{/if}
{#if icon == 'chevron-left'}
    {@html IconChevronLeft}
{/if}
{#if icon == 'chevron-right'}
    {@html IconChevronRight}
{/if}
</div>