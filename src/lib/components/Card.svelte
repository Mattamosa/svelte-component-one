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
  
  <!-- Card layout -->
  <div>
    <img src={image} alt="Card Image">
    <h2>{heading}</h2>
    <p>{description}</p>
    <Button text={button1Text} type={button1Type} />
    <Button text={button2Text} type={button2Type} />
  </div>
  