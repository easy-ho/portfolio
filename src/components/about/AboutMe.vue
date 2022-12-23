<script>
export default {
	setup() {
		return {
			bios: [
				{
					id: 1,
					bio:
						'안녕하세요. 5년차 서버 개발자 이지호입니다.' 
				},
				{
					id: 2,
					bio:
						'',
				},
			],
		};
	},
};
</script>

<template>
	<div class="block sm:flex sm:gap-10 mt-10 sm:mt-20">
		<!-- About profile image -->
		<div class="w-full sm:w-1/4 mb-7 sm:mb-0">
			<img
				src="@/assets/images/profile.jpeg"
				class="rounded-xl w-96"
				alt=""
			/>
		</div>

		<!-- About details -->
		<div class="w-full sm:w-3/4 text-left">
			<p
				v-for="bio in bios"
				:key="bio.id"
				class="font-general-regular mb-4 text-ternary-dark dark:text-ternary-light text-lg"
			>
				{{ bio.bio }}
			</p>

			<div class="w-1/3 mt-5 float-left">
				<p class="mt-20 text-sky-700 text-3xl font-bold -apple-system">Skill</p>
				
				<p class="">Java</p>
				<div class="bg-gray-200 rounded-full dark:bg-gray-700">
					<div class="bg-red-600 text-xs font-medium text-blue-100 text-center p-0.5 leading-none rounded-full" style="width: 85%"> 85%</div>
				</div>
			</div>

			<div class="w-1/3 mt-5 ml-5 float-left">
				<p class="">docker</p>
				<div class="bg-gray-200 rounded-full dark:bg-gray-700">
					<div class="bg-green-600 text-xs font-medium text-blue-100 text-center p-0.5 leading-none rounded-full" style="width: 30%"> 30%</div>
				</div>
			</div>

			<div class="w-1/3 mt-5 float-left">
				<p class="">aws</p>
				<div class="bg-gray-200 rounded-full dark:bg-gray-700">
					<div class="bg-blue-600 text-xs font-medium text-blue-100 text-center p-0.5 leading-none rounded-full" style="width: 70%"> 70%</div>
				</div>
			</div>

			<div class="w-1/3 mt-5 ml-5 float-left">
				<p class="">spring</p>
				<div class="bg-gray-200 rounded-full dark:bg-gray-700">
					<div class="bg-yellow-600 text-xs font-medium text-blue-100 text-center p-0.5 leading-none rounded-full" style="width: 90%"> 90%</div>
				</div>
			</div>

		</div>
	</div>
</template>
