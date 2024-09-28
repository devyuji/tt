<script lang="ts">
  import torrentList from "./lib/torrentlist";
</script>

<main>
  <div class="container">
    <nav class="navbar">
      <ul>
        <li>
          <a
            href="https://github.com/devyuji/tt"
            target="_blank"
            rel="noopener noreferrer">Add / Edit</a
          >
        </li>
      </ul>
    </nav>
    <div class="info--container">
      <h1>List of torrent websites that work.</h1>
      <h2>** Make sure to use VPN when using torrent websites **</h2>
    </div>

    <div class="link--container">
      <ol>
        {#each torrentList as list (list.id)}
          <li>
            <a href={list.url} target="_blank" rel="noopener noreferrer"
              >{list.name}</a
            >
          </li>
        {/each}
      </ol>
    </div>

    <div class="information--container">
      <p>
        List will be updated regulary so that you get the right torrent website.
      </p>
    </div>
  </div>
</main>
