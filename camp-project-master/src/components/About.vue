<script setup>
import {ArrowRightIcon} from "@heroicons/vue/outline";

const skills = [
	{
		title: 'Web開發',
		description: '開發網頁、網站、網路應用程式。',
	},
	{
		title: 'AMC 8 台灣前5%',
		description: 'AMC 是全美數學競賽，數字代表可以參加的最高年級',
	},
	{
		title: 'AMC 12',
		description: '參與AMC 12並達到前25%將受邀參與AIME',
	},

]
</script>

<template>

	<section id="about" class="pt-32 md:px-16 bg-blue-200">
		<div class="flex flex-col md:flex-row justify-between items-center md:px-8 md:mb-4">
			<h1 class="text-2xl md:text-4xl text-white font-bold">
				關於我
			</h1>
			<button
				class="my-8 mr-3 border-b border-white pb-2 flex items-center text-xl text-white">
				所有經歷
				<ArrowRightIcon class="ml-1 w-5 h-5"/>
			</button>
		</div>
		<div class="flex flex-wrap justify-start">
			<div
				class="w-full md:w-1/3"
				v-for="skill in skills">

				<div
					class="px-10 sm:px-20 py-3 sm:py-6 shadow-lg w-11/12 mx-auto bg-white rounded z-20 relative">
					<h4 class="text-black font-extrabold text-lg text-left mb-2">{{ skill.title }}</h4>
					<p class="text-black text-lg text-left mb-2">{{ skill.description }}</p>
				</div>
			</div>
		</div>
	</section>
</template>