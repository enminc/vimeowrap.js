# vimeowrap.js

vimeowrap is an easy to use Vimeo player embedder that can be extended with plugins.

## Features
* Uses oEmbed so the embed code is always up to date
* Playlist support, play videos one after another
* Extendable with plugins

## Usage
### Basic
``` html
<div id="player"></div>
<script src="http://luwes.co/vimeowrap.js/vimeowrap.js"></script>
<script>
	vimeowrap('player').setup({
		urls: [
			'https://vimeo.com/user3709818'
		]
	});
</script>
```

### Carousel Plugin
``` html
<div id="player"></div>
<script src="http://luwes.co/vimeowrap.js/vimeowrap.js"></script>
<script src="http://luwes.co/vimeowrap.js/vimeowrap.carousel.js"></script>
<script>
	vimeowrap('player').setup({
		urls: [
			'https://vimeo.com/user3709818'
		],
		plugins: {
			'carousel': {}
		}
	});
</script>
```

## Configuration
<table>
<thead><tr>
	<th>parameter</th> <th>default</th> <th>description</th>
</tr></thead>
<tbody>
	<tr>
		<th>`urls`</th>
		<td></td>
		<td>(required) Array with the Vimeo URL's. User or video URL's are supported</td>
	</tr>
	<tr>
		<th>width</th>
		<td>480</td>
		<td>Width of the Vimeo player</td>
	</tr>
	<tr>
		<th>height</th>
		<td>280</td>
		<td>Height of the Vimeo player</td>
	</tr>
	<tr>
		<th>color</th>
		<td>00adef</td>
		<td>Specify the color of the video controls</td>
	</tr>
	<tr>
		<th>byline</th>
		<td>true</td>
		<td>Show the byline on the video</td>
	</tr>
	<tr>
		<th>title</th>
		<td>true</td>
		<td>Show the title on the video</td>
	</tr>
	<tr>
		<th>portrait</th>
		<td>true</td>
		<td>Show the user's portrait on the video</td>
	</tr>
	</tbody>
</table>