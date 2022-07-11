<script setup>
import {ArrowRightIcon, ChevronDoubleDownIcon} from '@heroicons/vue/solid'
</script>
<template>
	<section class="bg-blue-200 flex flex-col justify-center items-center md:px-20 min-h-screen">
		<div class="flex flex-col w-full py-12 px-4 lg:px-0 justify-center items-end">
			<p class="text-2xl text-black-800 font-medium">哈囉！我是<span class="text-black-400">王昱凱</span></p>
			<h1 class="text-5xl text-right text-black-800 mt-1 font-bold">
				一個即將出國的高中生
			</h1>
			<p class="text-lg text-black-600 font-regular pt-8">
				A senior high student about to go abroad.
			</p>
			<a
				href="#contact"
				class="mt-3 flex items-center text-xl text-black-600 font-regular pb-2">
				聯絡我
				<ArrowRightIcon class="ml-1 w-5 h-5"/>
			</a>
		</div>

		<a href="#activities" class="animate-bounce cursor-pointer">
			<chevron-double-down-icon class="w-16 h-16"/>
		</a>
	</section>
</template>
