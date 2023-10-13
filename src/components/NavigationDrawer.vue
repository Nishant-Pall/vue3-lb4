<template>
	<v-card>
		<v-layout>
			<v-navigation-drawer expand-on-hover rail>
				<v-list>
					<v-list-item
						prepend-avatar="https://randomuser.me/api/portraits/women/85.jpg"
						title="Sandra Adams"
						subtitle="sandra_a88@gmailcom"
					></v-list-item>
				</v-list>

				<v-divider></v-divider>

				<v-list density="compact" nav>
					<v-list-item
						prepend-icon="mdi-folder"
						title="Page 1"
						value="page1"
					></v-list-item>
					<v-list-item
						prepend-icon="mdi-account-multiple"
						title="Page 2"
						value="page2"
					></v-list-item>
					<v-list-item
						prepend-icon="mdi-star"
						title="Page 3"
						value="page3"
					></v-list-item>
				</v-list>
			</v-navigation-drawer>
		</v-layout>
	</v-card>
</template>
<script setup></script>
