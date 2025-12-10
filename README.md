# Alta Control for Umbrel

An Umbrel app package for [Alta Labs Control](https://www.alta.inc/control) - a self-hosted network controller for Alta Labs networking equipment.

## Installation

### Option 1: Community App Store (Recommended)

Add this repository as a community app store in Umbrel:

1. Open your Umbrel dashboard
2. Go to **Settings** > **App stores**
3. Click **Add app store**
4. Enter: `https://github.com/posix4e/alta-controller-umbrel`
5. Find "Alta Control" in the app store and install

### Option 2: Manual Installation

```bash
# SSH into your Umbrel
ssh umbrel@umbrel.local

# Clone this repo
git clone https://github.com/posix4e/alta-controller-umbrel.git

# Copy the app to Umbrel's app directory
cp -r alta-controller-umbrel/alta-control ~/umbrel/app-data/
```

## Configuration

After installation, access Alta Control at `https://umbrel.local:8444`

### Device Discovery

For automatic device discovery, your Alta Labs equipment must be on the same network as your Umbrel device.

### Firmware Requirements

- Access Points: firmware 2.0g or higher
- Switches: firmware 2.1c or higher

To update firmware without cloud setup, hold the reset button for 5 seconds while powering on the device.

## Ports

| Port | Description |
|------|-------------|
| 8444 | Web UI (HTTPS) |
| 6080 | Device communication |
| 6443 | Device communication (secure) |

## Support

- [Alta Labs Forum](https://forum.alta.inc)
- [Alta Labs Help Center](https://help.alta.inc)

## License

This Umbrel package is provided as-is. Alta Control is a product of [Alta Labs](https://www.alta.inc).
