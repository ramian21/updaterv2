<script lang="ts">
  import Card, {
    Content,
    PrimaryAction,
    Media,
    MediaContent,
  } from "@smui/card";

  let clicked = 0;
</script>

<div class="card-container">
  <Card>
    <PrimaryAction on:click={() => clicked++} style="padding:0 20px;">
      <Content>
        <b>winner's pools</b><br />
        sgg user 1<br />
        vs<br />
        sgg user 2
      </Content>
    </PrimaryAction>
  </Card>
</div>

<pre class="status">Clicked: {clicked}</pre>

<style>
  .card-container {
    width: fit-content;
  }
</style>
