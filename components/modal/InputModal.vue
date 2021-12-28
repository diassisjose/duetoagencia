<template>
    <b-row>
        <b-col>
            <b-form-input v-model="text" placeholder="Enter your name"></b-form-input>
            <div class="mt-2">Value: {{ text }}</div>
        </b-col>
    </b-row>
</template>