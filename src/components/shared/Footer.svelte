<script lang="ts">
  import Nav from "./Nav.svelte";
  import Social from "./Social.svelte";

  const year = (): string => {
    const today = new Date();
    return String(today.getFullYear());
  };
</script>

<footer>
  <Nav className="py-12 mt-2" />

  <div class="bg-brightPink h-2 my-2" />

  <div class="bg-bunting text-white pb-16 pt-20 px-1 md:px-0">
    <Social className="pb-8 md:pb-16" />
    <ul class="font-sans uppercase tracking-widest text-sm flex justify-center pb-14 font-bold flex-col md:flex-row text-center">
      <li class="md:border-r-1 border-white px-6 mb-2 md:leading-5 text-sm md:mb-5">
          <a href="/legal/privacy-policy" class="hover:text-gold">Privacy Policy</a>
      </li>
      <li class="md:border-r-1 border-white px-6 mb-2 md:leading-5 text-sm md:mb-5">
          <a href="/legal/terms-and-conditions" class="hover:text-gold">Terms and Conditions</a>
      </li>
      <li class="px-6 md:leading-5 text-sm mb-2 md:mb-5">
          <a href="/legal/disclaimers" class="hover:text-gold">Disclaimers</a>
      </li>
    </ul>

    <p class="font-sans text-xs tracking-wide uppercase text-center font-bold">
      Copyright &copy; {year()}.{' '}
      <a href="http://ahhacreative.com" target="_blank" class="hover:underline hover:text-gold block md:inline">
        Ah Ha Creative, LLC.
      </a>
      &nbsp;All Rights Reserved.
    </p>
  </div>
</footer>
