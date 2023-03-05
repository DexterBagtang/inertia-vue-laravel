<template>
    <nav class="bg-gray-800">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="flex items-center justify-between h-16">
        <div class="flex items-center">
            <a href="#" class="text-white text-2xl font-bold">Logo</a>
        </div>
        <div class="flex">
            <Link href="/" 
            :class="{'underline': $page.component ==='Home'}"
            class="text-gray-300 hover:bg-gray-700 hover:text-white px-3 py-2 rounded-md text-sm font-medium">Home</Link>
            <Link href="users" 
            :class="{'underline': $page.component ==='Users'}"
            class="text-gray-300 hover:bg-gray-700 hover:text-white px-3 py-2 rounded-md text-sm font-medium">Users</Link>
            <Link href="settings" 
            :class="{'underline': $page.component ==='Settings'}"
            class="text-gray-300 hover:bg-gray-700 hover:text-white px-3 py-2 rounded-md text-sm font-medium">Settings</Link>
            <Link href="settings" class="text-gray-300 hover:bg-gray-700 hover:text-white px-3 py-2 rounded-md text-sm font-medium">Logout</Link>
        </div>
        </div>
    </div>
    </nav>
</template>

<script>
import { Link } from '@inertiajs/vue3';
export default{
    components:{
        Link,
    }
}
</script>