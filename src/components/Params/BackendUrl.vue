<script setup lang="ts">
import { useParamsStore } from '@/stores/paramsStore';

const store = useParamsStore()
</script>

<template>
    <v-card title="Backend Url" class="params" color="secondary" subtitle="Recommend to build your own backend service">
        <v-text-field label="Backend Url" v-model="store.data.advancedParams.backendUrl"></v-text-field>
        <v-btn href="https://github.com/tindy2013/subconverter" color="button" id="btn">Backend
            repository</v-btn>
    </v-card>
</template>

<style scoped>
#btn {
    margin-bottom: 2vh;
}
</style>