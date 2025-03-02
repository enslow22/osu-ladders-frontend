<script>
    import { Trigger as SidebarTrigger } from "$lib/components/ui/sidebar/index.js";
    import { Separator } from "$lib/components/ui/separator/index";
    import AuthButton from "$lib/components/auth-button.svelte";

    export const svgSize = 45;
</script>

<div class="p-8 flex-1">
    <div class="max-w-4xl mx-auto">
        <h1 class="text-4xl font-bold mb-4">What is osu!Lab?</h1>
        <p class="text-2xl mb-2 italic leading-relaxed">
            osu!Lab attempts to recognize the achievements of the
            dedicated players who grind underrepresented and unorthodox playstyles, and to provide players with detailed data analytics about themselves and their friends.
        </p>

        <hr class="mb-4">

        <section class="mb-8">
            <h2 class="text-2xl font-semibold mb-2">How it works</h2>
            <p class="text-base">
                Your scores need to be fetched from Bancho first. This can be
                done by entering the queue at <a href="https://api.enslow.me" class="text-blue-500 hover:text-blue-700">my api</a>.
            </p>
        </section>

        <section class="mb-8">
            <h2 class="text-2xl font-semibold mb-2">
                After your scores are fetched
            </h2>
            <p class="text-base">
                The database automatically updates with any new scores you set (Thanks <a class="text-blue-500 hover:text-blue-700" href="https://github.com/MaxOhn/scores-ws">MaxOhn</a>!).
                You can head to your user profile to see some basic statistics about your scores.
            </p>
        </section>

        <section class="mb-8">
            <h2 class="text-2xl font-semibold mb-2">Tags</h2>
            <p class="text-base">
                There is a player tagging system in place to help categorize players. You can use this feature to create groups of players and calcualte group stats.
                For example, I created a tag for only <a class="text-blue-500 hover:text-blue-700" href="/tags/OR">Oregon Players</a>, and I can see basics stats for all my oomfies.
                <br>
                <br>
                With tags, you can also control the default score and mod filters for the leaderboards. For example, the <a class="text-blue-500 hover:text-blue-700" href="/tags/EZ">EZ tag</a> has a default filter to only look at scores with
                the Easy mod enabled. 
                <br><br>
                You can read more information about tags <a class="text-blue-500 hover:text-blue-700" href="/tags">here</a>.
            </p>
        </section>

        <section class="mb-8">
            <h2 class="text-2xl font-semibold mb-2">Contact</h2>
            <p class="text-base">
                Feel free to reach out to me at any of my socials at the bottom if you have any suggestions or questions!
            </p>
        </section>
    </div>
</div>
<footer class="h-16 flex items-center gap-7 justify-center pb-5">
    <a aria-label="my osu! profile" href="https://osu.ppy.sh/users/enslow">
        <svg class="fill-white hover:fill-pink-300 transition-colors duration-300 ease-in-out" width="{svgSize}" height="{svgSize}" viewBox="0 0 300 300">
            <path d="M75.1 181.4c-4.7 0-8.8-.8-12.3-2.3s-6.4-3.7-8.6-6.4c-2.3-2.7-4-5.9-5.2-9.6s-1.7-7.6-1.7-11.9.6-8.3 1.7-12c1.2-3.7 2.9-7 5.2-9.7s5.2-4.9 8.6-6.5 7.6-2.4 12.3-2.4 8.8.8 12.3 2.4 6.4 3.7 8.8 6.5c2.3 2.7 4 6 5.2 9.7 1.1 3.7 1.7 7.7 1.7 12s-.6 8.2-1.7 11.9-2.8 6.9-5.2 9.6c-2.3 2.7-5.2 4.9-8.8 6.4-3.4 1.6-7.6 2.3-12.3 2.3zm0-12.1c4.2 0 7.2-1.6 9-4.7s2.7-7.6 2.7-13.4-.9-10.3-2.7-13.4-4.8-4.7-9-4.7c-4.1 0-7.1 1.6-8.9 4.7s-2.7 7.6-2.7 13.4.9 10.3 2.7 13.4c1.8 3.2 4.8 4.7 8.9 4.7zm51.8-14.5c-4.2-1.2-7.5-3-9.8-5.3-2.4-2.4-3.5-5.9-3.5-10.6 0-5.7 2-10.1 6.1-13.4 4.1-3.2 9.6-4.8 16.7-4.8 2.9 0 5.8.3 8.6.8s5.7 1.3 8.6 2.4c-.2 1.9-.5 4-1.1 6.1s-1.3 3.9-2.1 5.5c-1.8-.7-3.8-1.4-5.9-2-2.2-.6-4.5-.8-6.8-.8-2.5 0-4.5.4-5.9 1.2s-2.1 2-2.1 3.8c0 1.6.5 2.8 1.5 3.5s2.4 1.3 4.3 1.9l6.4 1.9c2.1.6 4 1.3 5.7 2.2s3.1 1.9 4.3 3.2 2.1 2.8 2.8 4.7 1 4.2 1 6.8c0 2.8-.6 5.3-1.7 7.7-1.2 2.4-2.8 4.5-5 6.2-2.2 1.8-4.9 3.1-8 4.2-3.1 1-6.7 1.5-10.7 1.5-1.8 0-3.4-.1-4.9-.2s-2.9-.3-4.3-.6-2.7-.6-4.1-1c-1.3-.4-2.8-.9-4.4-1.5.1-2 .5-4.1 1.1-6.1.6-2.1 1.3-4.1 2.2-6 2.5 1 4.8 1.7 7 2.2s4.5.7 6.9.7c1 0 2.2-.1 3.4-.3s2.4-.5 3.4-1 1.9-1.1 2.6-1.9 1.1-1.8 1.1-3.1c0-1.8-.5-3.1-1.6-3.9s-2.6-1.5-4.5-2.1zm39.3-32.7c2.7-.4 5.3-.7 8-.7 2.6 0 5.3.2 8 .7v30.7c0 3.1.2 5.6.7 7.6s1.2 3.6 2.2 4.7c1 1.2 2.3 2 3.8 2.5s3.3.7 5.3.7c2.8 0 5.1-.3 7-.8v-45.4c2.7-.4 5.3-.7 7.9-.7s5.3.2 8 .7v55.8c-2.4.8-5.6 1.6-9.5 2.4s-8 1.2-12.3 1.2c-3.8 0-7.5-.3-11-.9s-6.6-1.9-9.3-3.8-4.8-4.8-6.3-8.5c-1.6-3.7-2.4-8.7-2.4-14.9v-31.3zm65.9 58c-.4-2.8-.7-5.5-.7-8.2s.2-5.5.7-8.3c2.8-.4 5.5-.7 8.2-.7s5.5.2 8.3.7c.4 2.8.7 5.6.7 8.2 0 2.8-.2 5.5-.7 8.3-2.8.4-5.6.7-8.2.7-2.8-.1-5.5-.3-8.3-.7zm-.4-80.7c2.9-.4 5.8-.7 8.6-.7 2.9 0 5.8.2 8.8.7l-1.1 54.9c-2.6.4-5.1.7-7.5.7-2.5 0-5.1-.2-7.6-.7z M150 0C67.2 0 0 67.2 0 150s67.2 150 150 150 150-67.2 150-150S232.8 0 150 0zm0 285c-74.6 0-135-60.4-135-135S75.4 15 150 15s135 60.4 135 135-60.4 135-135 135z"/>
        </svg>
    </a>
    
    <a aria-label="my github profile" href="https://github.com/enslow22">
        <svg class="fill-white hover:fill-pink-300 transition-colors duration-300 ease-in-out" width="{svgSize}" height="{svgSize}" viewBox="0 0 98 96">
            <path d="M48.854 0C21.839 0 0 22 0 49.217c0 21.756 13.993 40.172 33.405 46.69 2.427.49 3.316-1.059 3.316-2.362 0-1.141-.08-5.052-.08-9.127-13.59 2.934-16.42-5.867-16.42-5.867-2.184-5.704-5.42-7.17-5.42-7.17-4.448-3.015.324-3.015.324-3.015 4.934.326 7.523 5.052 7.523 5.052 4.367 7.496 11.404 5.378 14.235 4.074.404-3.178 1.699-5.378 3.074-6.6-10.839-1.141-22.243-5.378-22.243-24.283 0-5.378 1.94-9.778 5.014-13.2-.485-1.222-2.184-6.275.486-13.038 0 0 4.125-1.304 13.426 5.052a46.97 46.97 0 0 1 12.214-1.63c4.125 0 8.33.571 12.213 1.63 9.302-6.356 13.427-5.052 13.427-5.052 2.67 6.763.97 11.816.485 13.038 3.155 3.422 5.015 7.822 5.015 13.2 0 18.905-11.404 23.06-22.324 24.283 1.78 1.548 3.316 4.481 3.316 9.126 0 6.6-.08 11.897-.08 13.526 0 1.304.89 2.853 3.316 2.364 19.412-6.52 33.405-24.935 33.405-46.691C97.707 22 75.788 0 48.854 0z"/>
        </svg>
    </a >
    <a aria-label="my twitter profile" href="https://twitter.com/ensl0">
        <svg class="fill-white hover:fill-pink-300 transition-colors duration-300 ease-in-out" width="{svgSize}" height="{svgSize}" viewBox="0 0 248 204">
            <path d="M221.95 51.29c.15 2.17.15 4.34.15 6.53 0 66.73-50.8 143.69-143.69 143.69v-.04c-27.44.04-54.31-7.82-77.41-22.64 3.99.48 8 .72 12.02.73 22.74.02 44.83-7.61 62.72-21.66-21.61-.41-40.56-14.5-47.18-35.07 7.57 1.46 15.37 1.16 22.8-.87-23.56-4.76-40.51-25.46-40.51-49.5v-.64c7.02 3.91 14.88 6.08 22.92 6.32C11.58 63.31 4.74 33.79 18.14 10.71c25.64 31.55 63.47 50.73 104.08 52.76-4.07-17.54 1.49-35.92 14.61-48.25 20.34-19.12 52.33-18.14 71.45 2.19 11.31-2.23 22.15-6.38 32.07-12.26-3.77 11.69-11.66 21.62-22.2 27.93 10.01-1.18 19.79-3.86 29-7.95-6.78 10.16-15.32 19.01-25.2 26.16z"/>
        </svg>
    </a>
    <svg class="fill-white hover:fill-pink-300 transition-colors duration-300 ease-in-out" width="{svgSize}" height="{svgSize}" viewBox="0 -28.5 256 256">
        <path d="M216.856339,16.5966031 C200.285002,8.84328665 182.566144,3.2084988 164.041564,0 C161.766523,4.11318106 159.108624,9.64549908 157.276099,14.0464379 C137.583995,11.0849896 118.072967,11.0849896 98.7430163,14.0464379 C96.9108417,9.64549908 94.1925838,4.11318106 91.8971895,0 C73.3526068,3.2084988 55.6133949,8.86399117 39.0420583,16.6376612 C5.61752293,67.146514 -3.4433191,116.400813 1.08711069,164.955721 C23.2560196,181.510915 44.7403634,191.567697 65.8621325,198.148576 C71.0772151,190.971126 75.7283628,183.341335 79.7352139,175.300261 C72.104019,172.400575 64.7949724,168.822202 57.8887866,164.667963 C59.7209612,163.310589 61.5131304,161.891452 63.2445898,160.431257 C105.36741,180.133187 151.134928,180.133187 192.754523,160.431257 C194.506336,161.891452 196.298154,163.310589 198.110326,164.667963 C191.183787,168.842556 183.854737,172.420929 176.223542,175.320965 C180.230393,183.341335 184.861538,190.991831 190.096624,198.16893 C211.238746,191.588051 232.743023,181.531619 254.911949,164.955721 C260.227747,108.668201 245.831087,59.8662432 216.856339,16.5966031 Z M85.4738752,135.09489 C72.8290281,135.09489 62.4592217,123.290155 62.4592217,108.914901 C62.4592217,94.5396472 72.607595,82.7145587 85.4738752,82.7145587 C98.3405064,82.7145587 108.709962,94.5189427 108.488529,108.914901 C108.508531,123.290155 98.3405064,135.09489 85.4738752,135.09489 Z M170.525237,135.09489 C157.88039,135.09489 147.510584,123.290155 147.510584,108.914901 C147.510584,94.5396472 157.658606,82.7145587 170.525237,82.7145587 C183.391518,82.7145587 193.761324,94.5189427 193.539891,108.914901 C193.539891,123.290155 183.391518,135.09489 170.525237,135.09489 Z"/>
    </svg>
</footer>

<style>
    /* Add your styles here */
</style>
