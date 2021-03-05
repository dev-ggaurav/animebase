<template>
  <div class="wrapper">
      <div class="spinner"></div>

      <label class="switch">
        <input type="checkbox" class="checkbox">
        <span class="toggle-thumb">
          <svg xmlns="http://www.w3.org/2000/svg" width="36" height="36" viewBox="0 0 24 24" style="fill:#4ADE80;transform:;-ms-filter:"><path d="M10 15.586L6.707 12.293 5.293 13.707 10 18.414 19.707 8.707 18.293 7.293z"></path></svg>
          <svg xmlns="http://www.w3.org/2000/svg" width="36" height="36" viewBox="0 0 24 24" style="fill:#F87171;transform:;-ms-filter:"><path d="M16.192 6.344L11.949 10.586 7.707 6.344 6.293 7.758 10.535 12 6.293 16.242 7.707 17.656 11.949 13.414 16.192 17.656 17.606 16.242 13.364 12 17.606 7.758z"></path></svg>
        </span>
      </label>
  </div>
</template>

<script>
export default {

}
</script>

<style>
    .spinner {
      width: 64px;
      height: 64px;
      border: 8px solid;
      border-color: #3d5af1 transparent #3d5af1 transparent;
      border-radius: 50%;
      animation: spin 1.2s linear infinite;
    }

    @keyframes spin {
      0% {
        transform: rotate(0deg);
      }

      100% {
        transform: rotate(360deg);
      }
    }


    .switch {
      display: inline-block;
      width: 60px;
      height: 34px;
      position: relative;
    }

    .checkbox {
      opacity: 0;
      width: 0;
      height: 0;
    }

    .toggle-thumb {
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      display: flex;
      justify-content: space-between;
      align-items: center;
      background-color: #475569;
      border-radius: 40px;
      cursor: pointer;
    }

    .toggle-thumb:before {
      content: "";
      height: 26px;
      width: 26px;
      position: absolute;
      left: 4px;
      bottom: 4px;
      border-radius: 50%;
      background-color: #E2E8F0;
      transition: .4s all ease;
    }

    input:checked+.toggle-thumb:before {
      transform: translateX(26px);
    }

</style>