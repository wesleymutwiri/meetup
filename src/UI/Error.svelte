<script>
    import Modal from './Modal.svelte';
    export let message;

    function clearError() {
        error = null;
    }
</script>

<Modal title="An error occured" on:cancel={clearError}>
    <p>{message}</p>
</Modal>