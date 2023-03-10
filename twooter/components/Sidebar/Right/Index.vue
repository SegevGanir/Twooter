<template>
    <div class="flex flex-col">
        
        <!--Preview Card : What's Happening-->
        <SidebarRightPreviewCard title="What's Happening" >

            <SidebarRightPreviewCardItem v-for="whatsHappening in whatsHappeningItems">
                <div>

                    <h2 class="font-bold text-gray-800 text-md dark:text-white">{{ whatsHappening.title }}</h2>
            
                    <p class="text-xs text-gray-400">
                        {{ whatsHappeningItems.count }}
                    </p>
                </div>
            </SidebarRightPreviewCardItem>

        </SidebarRightPreviewCard>

        

        <!--Preview Card : Who to follow?-->
        <SidebarRightPreviewCard title="Who to follow?">
            <SidebarRightPreviewCardItem v-for="whoToFollow in whoToFollowItems">
                <div class="flex flex-row justify-between p-2">
                    <div class="flex flex-row">
                        <img class="w-10 h-10 rounded-full"   src="" alt="">
                    </div>
                </div>
            </SidebarRightPreviewCardItem>
        </SidebarRightPreviewCard>
        
    </div>
</template>
<script setup>

const whatsHappeningItems = ref([
    {
        title: 'SpaceX',
        count: '18.8k Tweets'
    },
    {
        title: '#CodingIsFun',
        count: '8.8k Tweets'
    },
    {
        title: '#artforall',
        count: '1.8k Tweets'
    },

])

const whoToFollowItems = ref([
    {
        name: 'Joe Biden',
        handle: '@PrezzyWezzy'
        
    }
])


</script>
