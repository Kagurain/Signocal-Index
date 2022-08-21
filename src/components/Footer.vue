<script setup>
import { ref } from "vue";
import Github from "./img/Github.vue";

const date = ref();
date.value = new Date().getFullYear();

window.onload = function () {
	document.oncontextmenu = function () {
		return false;
	};
};
</script>

<template>
	<footer>
		<div class="fixed bottom-0 left-0 right-0 p-5 text-zinc-500 font-light text-sm flex flex-row justify-center items-center">
			<span>
				Copyright ©
				{{ date }}
				<a class="hover:underline hover:underline-offset-1" href="https://zzlz.gsxt.gov.cn/businessCheck/viewPdfImage?licence13=92350212MA8W1WFW01" target="_blank" rel="noopener noreferrer">厦门市同安区辞寒网络工作室</a>
				版权所有
			</span>
			<span class="flex justify-center items-center">
				<a class="rounded-full transition-all duration-500 hover:scale-150" href="https://github.com/Kagurain/Signocal-Index" target="_blank" rel="noopener noreferrer">
					<Github />
				</a>
			</span>
		</div>
	</footer>
</template>
