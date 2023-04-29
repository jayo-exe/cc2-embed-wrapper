# Steam Embed Wrapper for Crowd Control 2.0 Beta
Crowd Control 2.0 menu, Stream and Chat -- all on one convenient, standalone page.

Provide your viewers with a way to use Crowd Control more comfortably, with your effects menu, stream feed, and chat all on the same page in a familiar arrangement.  Currently only supports Twitch streams.

One small, standalone HTML file that relies on zero external libraries means that this can be deployed on virtually _any_ hosting service!

## Installation
The wrapper is available in two flavours: 
- **Universal**: The wrapper can show anyone's stream (based on the URL), requires no configuration, but requires your link to include your details in a specific structure.
- **Custom**: The wrapper always shows the stream you specify, requires no extra bits in your URL, but requires you to modify the file to include your stream details.

### Universal Wrapper
- Clone the repository, or grab your file of choice from the Releases page.  The wrappers are provided in both pretty-printed and minified versions.
- Rename the file to whatever you'd like and upload it to your web host, or otherwise get the resulting HTML/CSS/JS into your existing architecture.
- That's it!  You can see the embed page for any given stream by going to `https://your-site.com/your-chosen-path.html/#/twitch/abcdefg-1234567` where:
  - `abcdefg` is your twitch channel name 
  - `1234567` is your Crowd Control Origin ID (that number at the end of your Extension URL)
  
### Custom Wrapper
- Clone the repository, or grab your file of choice from the Releases page.  The wrappers are provided in both pretty-printed and minified versions.
- Modify your chosen file to provide your stream details.  You'll find these values at the beginning of the `<script>` tag:
```
const twitchName = "your_channel_name";
const originId = "1234567" //Your Origin ID
```
- Rename the file to whatever you'd like and upload it to your web host, or otherwise get the resulting HTML/CSS/JS into your existing architecture.
- That's it!  You can see the embed page for your configured stream by going to `https://your-site.com/your-chosen-path.html`
