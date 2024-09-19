<script>
    import Button from './Button.svelte';
  
    export let image;
    export let heading;
    export let description;
    export let button1Text;
    export let button2Text;
    export let button1Type;
    export let button2Type;
  </script>
  
  <section class="m-3 w-[23.438rem] h-[50.75rem] rounded-[2rem] bg-white">
    <section class="bg-layer2gray w-full h-full flex items-center justify-center rounded-[2rem]">
      <div class="w-[20.438rem] rounded-[2rem] bg-white">
        <!-- card-image -->
        <div class="rounded-t-2xl">
          <img class="rounded-t-2xl w-full h-48 object-cover" src={image} alt="Abstract Image" />
        </div>
        <!-- card-content -->
        <div class="w-full bg-white text-black p-6 rounded-b-2xl flex flex-col justify-center items-center">
          <h4 class="text-2xl font-bold text-black mb-3 text-center">
            {heading}
          </h4>
          <p class="text-base font-light text-gray-500 mb-4">{description}</p>
          
          <!-- Button component -->
          <Button text={button1Text} type={button1Type} />
          <Button text={button2Text} type={button2Type} />
        </div>
      </div>
    </section>
  </section>
  