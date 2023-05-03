<script lang="ts">
  export let name: string;
</script>

<div class="tile-box">
  <div class="icon-container">
    <img
      src="https://cdn4.iconfinder.com/data/icons/social-media-icons-the-circle-set/48/twitter_circle-512.png"
      alt="twitter"
      width="24"
      height="24"
    />
  </div>
  <p class="name">{name}</p>
</div>

<style>
  .tile-box {
    /* border: 1px solid red; */
    width: 112px;
    height: 112px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .tile-box:hover {
    cursor: pointer;
    background-color: rgba(255, 255, 255, 0.1);
    border-radius: 4px;
  }
  .icon-container {
    width: 48px;
    height: 48px;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: rgb(87, 52, 129);
    margin-bottom: 16px;
  }
  .name {
    color: white;
    font-size: 13px;
  }
</style>
