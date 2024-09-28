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
      <h2>
        ** Don't be a pirate without a patch! Use a VPN to sail the seas safely.
        **
      </h2>
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
  </div>
</main>
