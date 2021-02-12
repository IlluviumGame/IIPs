# IIPs [![Discord](https://img.shields.io/discord/760344898200666112.svg?color=768AD4&label=discord&logo=https%3A%2F%2Fdiscordapp.com%2Fassets%2F8c9701b98ad4372b58f13fd9f65f966e.svg)](https://discordapp.com/channels/760344898200666112/) [![Twitter Follow](https://img.shields.io/twitter/follow/illuviumio.svg?label=illuviumio&style=social)](https://twitter.com/illuviumio)

### WORK IN PROGRESS

Illuvium Improvement Proposals (IIPs) describe standards for the Illuvium platform, including core protocol specifications, client APIs, and contract standards.


# Contributing

1.  Review [IIP-1](iips/iip-1.md).
2.  Fork the repository by clicking "Fork" in the top right.
3.  Add your IIP to your fork of the repository. There is a [template IIP here](iip-x.md).
4.  Submit a Pull Request to Illuvium's [IIPs repository](https://github.com/IlluviumGame/IIPs).

Your first PR should be a first draft of the final IIP. It must meet the formatting criteria enforced by the build (largely, correct metadata in the header). An editor will manually review the first PR for a new IIP and assign it a number before merging it. 

If your IIP requires images, the image files should be included in a subdirectory of the `assets` folder for that IIP as follow: `assets/iip-X` (for iip **X**). When linking to an image in the IIP, use relative links such as `../assets/iip-X/image.png`.

When you believe your IIP is mature and ready to progress past the WIP phase, you should ask to have your issue added to the next governance call where it can be discussed for inclusion in a future platform upgrade. If the community agrees to include it, the IIP editors will update the state of your IIP to 'Approved'.

# IIP Statuses

- **WIP** - a IIP that is still being developed.
- **Proposed** - a IIP that is ready to be reviewed in a governance call.
- **Approved** - a IIP that has been accepted for implementation by the Illuvium community.
- **Implemented** - a IIP that has been released to mainnet.
- **Rejected** - a IIP that has been rejected.

# Validation

IIPs must pass some validation tests. The IIP repository ensures this by running tests using [html-proofer](https://rubygems.org/gems/html-proofer) and [iip_validator](https://rubygems.org/gems/iip_validator).

It is possible to run the IIP validator locally:

```
gem install iip_validator
iip_validator <INPUT_FILES>
```
