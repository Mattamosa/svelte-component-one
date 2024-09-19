<script>
    export let text;
    export let type = "primary"; // default type is primary
  
    let buttonClass = 
      type === "primary"
        ? "bg-btnColor text-white"
        : type === "secondary"
        ? "text-btnColor border border-btnColor"
        : "text-gray-500 cursor-not-allowed";
  </script>
  
  <button class="w-[18.563rem] h-12 rounded-[3rem] text-base font-medium mb-2 cursor-pointer {buttonClass}">
    {text}
  </button>
  
  <style>
    .bg-btnColor {
      background-color: #1d4ed8;
    }
    .text-btnColor {
      color: #1d4ed8;
    }
  </style>