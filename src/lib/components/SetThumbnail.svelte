<script lang="ts">
  import Card, {
    Content,
    PrimaryAction,
    Media,
    MediaContent,
  } from "@smui/card";

  export let roundTitle : string;
  export let player1Tag : string;
  export let player2Tag : string;
</script>

<div class="card-container">
  <Card style="margin: 10px;">
    <PrimaryAction style="padding:0 20px;">
      <Content>
        <b>{roundTitle}</b><br />
        {player1Tag} <br />
        vs<br />
        {player2Tag}
      </Content>
    </PrimaryAction>
  </Card>
</div>

<style>
  .card-container {
    width: fit-content;
  }
</style>
