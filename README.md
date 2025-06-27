# Motivational Quotes Plugin for Dify

**Author:** amandevelops  
**Version:** 0.0.1  
**Type:** tool

## Description

Motivational Quotes is a Dify plugin that provides random inspirational quotes to uplift and motivate users during conversations. The plugin includes a collection of motivational quotes from famous individuals like Steve Jobs, Albert Einstein, Eleanor Roosevelt, and many others.

## Features

- Random delivery of motivational quotes
- A collection of 25+ hand-picked inspirational quotes

## Installation

### Prerequisites

- A Dify account with access to plugin management
- Dify instance (cloud or self-hosted)

### Steps to Install

1. Log in to your Dify account
2. Navigate to the "Plugins" section
3. Search for "Motivational Quotes" in the marketplace
4. Click "Install" to add the plugin to your Dify instance
5. No additional configuration or API keys are required

## Usage

### In Dify Applications

Once installed, you can use the plugin in your Dify applications by:

1. Go to your application settings
2. Navigate to the "Tools" tab
3. Enable the "Motivational Quotes" plugin
4. Save your changes

### Example Response

When triggered, the plugin will respond with a random quote like:

> "The only way to do great work is to love what you do. - Steve Jobs"


### Running the Plugin Locally

Start the plugin for local development:

```bash
python -m main
```

### Modifying the Quotes Collection

To add or modify the quotes, edit the `tools/motivational-quotes.py` file:

```python
def __init__(self):
    super().__init__()
    self.quotes = [
        # Add or modify quotes here
        "Your new quote here. - Author Name",
        # ...
    ]
```

### Packaging the Plugin

To package the plugin for distribution:

```bash
dify-plugin plugin package ./
```

This will create a `plugin.difypkg` file that can be submitted to the Dify Marketplace.


