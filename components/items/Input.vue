<template>
    <div class="flex h-screen w-full bg-gray-700">
        <div class="m-auto w-full px-5 md:w-1/3">
            <div class="pl-1 text-white font-medium text-2xl tracking-
wide text-center">
                <form>
                    <div class="my-2">
                        <inputElement
                            :labelName="'EMAIL'"
                            :labelId="'email'"
                            :inputType="'email'"
                            :model="email"
                            @input="email = $event"
                            :disabled="false"
                        /> 
                    </div>
                    <div class="my-2">
                        <inputElement
                            :labelName="'PASSWORD'"
                            :labelId="'password'"
                            :inputType="'password'"
                            :model="password"
                            @input="password = $event"
                            :disabled="false"
                        />
                    </div>
                    <button type="button" class="
                        transition
                        duration-500
                        ease-in-out
                        bg-blue-600
                        rounded-xs
                        w-full
                        py-3
                        text-white
                        font-sans
                        font-bold
                        tracking-wide
                        hover:bg-blue-700
                        hover:text-gray-400
                        active:outline-none
                        focus:outline-none
                        "> SIGN IN 
                    </button>
                </form>
            </div>
        </div>
    </div>
</template>

<script>
import Logo from '~/components/items/Logo.vue'
import InputElement from "~/components/items/Input.vue";

export default {
    components:{
        Logo
        InputElement
    },
        data: function(){
            return{
                email: "",
                password: ""
    }
}
</script>

