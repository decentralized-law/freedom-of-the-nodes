# Website Integration Guide

This guide explains how to add the Freedom of the Nodes principle to your website.

## Basic Implementation

1. **Download the file**
   - Download the `FreedomOfTheNodesFrontEnd.html` file from this repository's `frontend` directory

2. **Add to your website**
   - Copy the HTML code from the file
   - Paste it into any page on your website where you want to display the Freedom of the Nodes principle
   - **Important:** Many standard content management systems, such as WordPress, require a specific HTML embedding approach (see Website Builder Implementation below)

3. **Key customization points**
   - Contract address: The file is pre-configured with the official Ethereum contract address `0x4A4b427c7C5417e6C50999ab546064b751e0365b`
   - RPC URL: Modify the `rpcUrl` variable to use your preferred Ethereum node provider if needed
   - Styling: Adjust the `titleStyle` and `textStyle` variables to match your website's design

### Website Builder Implementation

When using website builders such as WordPress, Wix, Squarespace, or Shopify, you might need to use their specific HTML embedding features to add this code to your site. Look for options like "Custom HTML," "HTML Embed," "Code Block," or similar functionality in your website builder's interface. Make sure you're pasting the code in HTML mode rather than visual/text mode for proper functionality.

## Configuration Options

### Contract Address

```javascript
// The official deployed contract address
const contractAddress = "0x4A4b427c7C5417e6C50999ab546064b751e0365b";
```

### Ethereum Network URL

```javascript
// Ethereum Mainnet (production)
const rpcUrl = "https://ethereum.publicnode.com";
```

You can use any Ethereum mainnet RPC provider of your choice, including your own node if you have one.

## Alternative Integration Methods

### IPFS Integration

If you prefer to load the Freedom of the Nodes from IPFS instead of directly from the Ethereum blockchain, you can use the following IPFS CID:

```
bafkreigrzc2rxfwsklzr3ayrqwxnnubsmmzgwrotjhojpny4lxxi6rmyvi
```

You can access this through any IPFS gateway, for example:
```
https://ipfs.io/ipfs/bafkreigrzc2rxfwsklzr3ayrqwxnnubsmmzgwrotjhojpny4lxxi6rmyvi
```

or

```
https://gateway.pinata.cloud/ipfs/bafkreigrzc2rxfwsklzr3ayrqwxnnubsmmzgwrotjhojpny4lxxi6rmyvi
```

### Direct PDF Embedding

You can also directly embed the PDF version of the Freedom of the Nodes principle if you prefer a static implementation that doesn't rely on blockchain connectivity.

## Troubleshooting

If you encounter issues:

1. **Contract not loading**: Check that your website allows external connections to Ethereum nodes
2. **Content display issues**: Verify that your CMS or website builder properly displays HTML and JS content
3. **Styling conflicts**: Adjust the styling variables to avoid conflicts with your website's CSS

## That's it!

The HTML file is self-contained with all necessary code to fetch and display the Freedom of the Nodes principle. No additional files or dependencies need to be installed on your server.
