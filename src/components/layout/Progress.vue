<template>
	<div class="lg:flex lg:items-start lg:justify-between">
		<section dir="ltr" class="p-5 m-5 bg-white rounded-lg sm:mt-0 front lg:ml-0">
			<h1 style="direction: rtl" class="mb-3 text-xl font-bold">فرانت_اند</h1>
			<div
				class="space-y-2 tracking-tighter sm:flex sm:items-start sm:space-y-0 sm:space-x-10 lg:block lg:space-x-0 lg:space-y-2"
			>
				<div class="space-y-2 sm:w-1/2 lg:w-full">
					<!-- Vue -->
					<div class="flex items-center justify-between space-x-5">
						<h3>Vue</h3>
						<div
							class="
								w-full
								bg-gray-200
								rounded-full
								h-2.5
								dark:bg-gray-700
								w-3/4
							"
						>
							<div
								class="bg-blue-600 h-2.5 rounded-full"
								style="width: 55%"
							></div>
						</div>
					</div>
					<!-- Tailwind -->
					<div class="flex items-center space-x-3">
						<h3 class="sm:pr-3.5 lg:pr-6">Tailwind</h3>
						<div class="w-full bg-gray-200 rounded-full h-2.5 dark:bg-gray-700">
							<div
								class="bg-blue-600 h-2.5 rounded-full"
								style="width: 75%"
							></div>
						</div>
					</div>
					<!-- Css -->
					<div class="flex items-center justify-between space-x-5">
						<h3>Css</h3>
						<div
							class="
								w-full
								bg-gray-200
								rounded-full
								h-2.5
								dark:bg-gray-700
								w-3/4
							"
						>
							<div
								class="bg-blue-600 h-2.5 rounded-full"
								style="width: 65%"
							></div>
						</div>
					</div>
				</div>
				<div class="space-y-2 sm:w-1/2 lg:w-full">
					<!-- Nuxt -->
					<div class="flex items-center justify-between space-x-5">
						<h3>Nuxt</h3>
						<div
							class="
								w-full
								bg-gray-200
								rounded-full
								h-2.5
								dark:bg-gray-700
								w-3/4
							"
						>
							<div
								class="bg-blue-600 h-2.5 rounded-full"
								style="width: 45%"
							></div>
						</div>
					</div>
					<!-- Pinia -->
					<div class="flex items-center justify-between space-x-5">
						<h3>Pinia</h3>
						<div
							class="
								w-full
								bg-gray-200
								rounded-full
								h-2.5
								dark:bg-gray-700
								w-3/4
							"
						>
							<div
								class="bg-blue-600 h-2.5 rounded-full"
								style="width: 35%"
							></div>
						</div>
					</div>
				</div>
			</div>
		</section>
		<section
			dir="ltr"
			class="hidden p-5 m-5 bg-white rounded-lg lg:block sm:mt-0 sm:mr-0 sm:w-1/3 lg:hidden"
		>
			<h1 style="direction: rtl" class="mb-3 text-xl font-bold">طراحی</h1>
			<div class="space-y-2 tracking-tighter">
				<!-- Figma -->
				<div class="flex items-center justify-between space-x-5">
					<h3 class="pr-5">Figma</h3>
					<div
						class="w-full bg-gray-200 rounded-full h-2.5 dark:bg-gray-700 w-28"
					>
						<div
							class="bg-blue-600 h-2.5 rounded-full"
							style="width: 35%"
						></div>
					</div>
				</div>
				<!-- Photoshop -->
				<div class="flex items-center space-x-3">
					<h3>Photoshop</h3>
					<div class="w-full bg-gray-200 rounded-full h-2.5 dark:bg-gray-700">
						<div
							class="bg-blue-600 h-2.5 rounded-full"
							style="width: 15%"
						></div>
					</div>
				</div>
			</div>
		</section>
	</div>
</template>

<style scoped>
@media (min-width: 768px) {
	.front {
		width: 25.5rem;
	}
}
</style>