<script>
  // make dynamic date to be added to footer
  let date = new Date().getFullYear();
</script>

<footer>
    <hr class="my-6 border-blueGray-300" />
    <div class="flex flex-wrap items-center md:justify-between justify-center">
      <div class="w-full md:w-4/12 px-4 mx-auto text-center">
        <div class="text-sm text-blueGray-500 font-semibold py-1">
          Copyright © {date} Notus Svelte by
          <a
            href="https://www.creative-tim.com?ref=ns-footer"
            class="text-blueGray-500 hover:text-blueGray-800"
          >
            Creative Tim
          </a>
          .
        </div>
      </div>
    </div>

</footer>
