<script>
    import '../app.css';
    import Ducklogo from '../images/ducklogo.jpg';
</script>

<nav class="bg-gray-800">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="flex items-center justify-center h-16">
            <div class="flex items-center">
                <div class="flex-shrink-0">
                    <img class="h-8 w-8" src="{Ducklogo}" alt="Logo">
                </div>
                <div class="hidden md:block">
                    <div class="ml-4 flex items-baseline space-x-4">
                        <a href="/" class="text-gray-300 hover:bg-gray-700 hover:text-white px-3 py-2 rounded-md text-sm font-medium">Home</a>
                        <a href="/about" class="text-gray-300 hover:bg-gray-700 hover:text-white px-3 py-2 rounded-md text-sm font-medium">About</a>
                        <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white px-3 py-2 rounded-md text-sm font-medium">Projects</a>
                        <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white px-3 py-2 rounded-md text-sm font-medium">Contact</a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</nav>



<slot />


<!-- 오른쪽 하단에 고정되어 있는 버튼이 있고 클릭 시 웹페이지 최상단으로 가는 기능을 넣어줘-->
<button class="fixed bottom-0 right-0 m-4 bg-gray-800 text-white p-4 rounded-md" on:click={() => window.scrollTo({ top: 0, behavior: 'smooth' })}>
    <svg class="h-6 w-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 10l7-7m0 0l7 7m-7-7v18"></path>
    </svg>
</button>



<footer class="bg-gray-800 text-white text-center py-4">
    <p class="text-sm font-mono">2024 Duck page<br> Made by <a href="https://github.com/DoDAON", target="_blank">DoDAON</a></p>
</footer>

<style>
    @media (max-width: 640px) {
        .flex {
            flex-wrap: wrap;
        }
    }
    :global(body){
        background-color: black;
    }
</style>
