<script>
  import Nav from './components/Navbar.svelte';
	import Header from './components/Header.svelte';
	import Footer from './components/Footer.svelte';
  import Modal from './components/Modal.svelte';

let showModal = false;
export let segment;
  // import MOCK_DATA from './Data/data';

// import QuickSearchBar from "svelte-quicksearch-bar@latest";
// const onPick = ({detail}) => selectedOption = detail;
// let options = [
// 	{label: "Example", link: "/"},
// 	{label: "Search with fuzzy", link: "/also"},
// 	{label: "Bolds the text", link: "/in"},
// 	{label: "Other example", link: "/the-link"},
// ];
// let inputEl;
// let selectedOption;
// let value;
</script>

<!-- <Navbar title="My App" backLink="Back" large titleLarge="Large Title">
  <a href="#" slot="left">Left Link</a>
  <a href="#" slot="right">Right Link</a>
  <div slot="before-inner">Before Inner</div>
  <div slot="after-inner">After Inner</div>
  <div>Default slot</div>
</Navbar>

<div class="navbar">
  <div class="navbar-bg"></div>
  <div>Before Inner</div>
  <div class="navbar-inner">
    <div class="left">
      <a href="#">Left Link</a>
    </div>
    <div class="title">My App</div>
    <div class="right">
      <a href="#">Right Link</a>
    </div>
    <div>Default slot</div>
  </div>
  <div>After Inner</div>
</div> -->

<Nav {segment}/>
<!-- <Header /> -->

<!-- <QuickSearchBar {options} {inputEl} bind:value on:pick={onPick} keys={['label', 'link']}>
  <span slot="input">
    <input type="text" bind:value bind:this={inputEl} />
  </span>
  <span slot="item" let:option>
    {@html option.html.label}
    <span class="secondary-text">
      {@html option.html.link}
    </span>
  </span>
</QuickSearchBar>

<p>Press CTRL + K to open (the window has to be in focus)</p>
<p>Selected: {JSON.stringify(selectedOption)}</p> -->

<main>
  <h1> Tools with missing fields - </h1>


  <button on:click="{() => showModal = true}">
    Tool name: vdfbgd
    Discription: dfbgbf 
    vfdgbjnnnnnnnnnnnnnnn
  </button>
  
  {#if showModal}
    <Modal on:close="{() => showModal = false}">
      <h2 slot="header">
        modal
        <small><em>adjective</em>  mod·al \ˈmō-dəl\</small>
      </h2>
  
      <ol class="definition-list">
        <li>of or relating to modality in logic</li>
        <li>containing provisions as to the mode of procedure or the manner of taking effect —used of a contract or legacy</li>
        <li>of or relating to a musical mode</li>
        <li>of or relating to structure as opposed to substance</li>
        <li>of, relating to, or constituting a grammatical form or category characteristically indicating predication</li>
        <li>of or relating to a statistical mode</li>
      </ol>
  
      <a href="https://www.merriam-webster.com/dictionary/modal">merriam-webster.com</a>
    </Modal>
  {/if}
  








</main>
<Footer />

<style>
	main{
    /* background: #ffffff; */
    width: 100%;
    max-width: 960px;
    margin: 40px auto;
  }

  /* .secondary-text {
		font-size: 0.7em;
		color: purple;
	}
	input {
		width: 100%;
	} */

</style>