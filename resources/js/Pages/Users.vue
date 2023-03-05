<template>
    Users
    <Nav></Nav>

    <table class="min-w-full divide-y divide-gray-200">
        <tr>
            <th class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">Name</th>
            <th class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider" >Email</th>
            <th class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider"></th>
        </tr>
        <tr class="bg-white divide-y divide-gray-200">
            <td>Dexter</td>
            <td>dexter@gmail.com</td>
            <td>
                <button class="border bg-blue-300 rounded-lg text-blue-700 py-1 px-3">Action</button>
            </td>
        </tr>
    </table>

    <div style="margin-top: 1000px">
        <p>The current time is {{ time }}</p>
        <Link href="/users" class="text-blue-500" preserve-scroll>Refresh</Link>
    </div>


</template>


<script>
import Nav from '@/Pages/Shared/Nav.vue';
import {Link} from '@inertiajs/vue3';
export default{
    components:{
        Nav,
        Link,
    },
    props:{
        time:String,
    }
}
</script>