<script>
    export let text;
    export let type = "primary"; // Default type is primary
  
    // Button classes based on the type
    let buttonClass = 
      type === "primary" // Switch to 'secondary' to see the changes
        ? "bg-btnColor text-white hover:bg-btnColor2"
        : type === "secondary"
        ? "text-btnColor hover:bg-btnColor2"
        : "text-btnColor cursor-not-allowed";
  </script>
  
  <button class={`w-full h-12 rounded-full text-base font-medium mb-2 ${buttonClass}`}>
    {text}
  </button>
  
  