<template>
    <ul class="chat">
        <li class="left clearfix" v-for="message in messages">
            <div class="chat-body clearfix">
                <div class="strong">
                    {{ message.user.name }}
                </div>
            </div>
            <p>
                {{ message.message }}
            </p>
        </li>
    </ul>
</template>

<script>
    export default {
        props: ['messages']
    };
</script>