<script>
export default {
    data() {
        return {
        navBarLinks : [
            {
                id: '1',
                label: 'Characters',
                url:'#',
                active: false
            },
                {
                id: '2',
                label: 'Comics',
                url:'#',
                active: true
            },
            {
                id: '3',
                label: 'Movies',
                url:'#',
                active: false
            },
            {
                id: '4',
                label: 'TV',
                url:'#',
                active: false
            },
            {
                id: '5',
                label: 'Games',
                url:'#',
                active: false
            },
            {
                id: '6',
                label: 'Collectibles',
                url:'#',
                active: false
            },
            {
                id: '7',
                label: 'Videos',
                url:'#',
                active: false
            },
            {
                id: '8',
                label: 'Fans',
                url:'#',
                active: false
            },
            {
                id: '9',
                label: 'News',
                url:'#',
                active: false
            },
            {
                id: '10',
                label: 'Shop',
                url:'#',
                active: false
            },
            
        ]
        }
    }
}
</script>


<template>
    <header>
        <div class="logo">
            <img src="../assets/img/dc-logo.png">
        </div>
        <div class="navbar">
            <nav>
                <ul>
                    <li v-for="navBarItem in navBarLinks" :key="navBarItem.id" class="{active : navBarItem.active}">
                        <a :href="navBarItem.url">
                            {{ navBarItem.label }}
                        </a>
                    </li>
                    
                </ul>
            </nav>
        </div>
    </header>
</template>

<style scoped lang="scss">
a{
    color:rgb(69, 66, 66);
    text-decoration: none;
}
</style>