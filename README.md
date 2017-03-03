# startuptime.vim

![startuptime](https://cloud.githubusercontent.com/assets/111942/23541408/35607a3e-ffb5-11e6-9bf8-1e59b8ae06ef.png)

Everybody knows that 1ms could mean the difference between life and death in
Vim.  This plugin breaks down the output of `--startuptime` so you can zero in
on the scripts that are stealing dozens of your milliseconds each time Vim is
started.  You won't even need to leave the comfort of Vim.


# Requirements

- Not Windows :-(
- Command line programs:
  - `script` (typescript)
  - `ps`


# Usage

Use the command `:StartupTime` to get an averaged startup profile.  By default,
it collects 10 samples.  Since it's very important we get an accurate profile,
we can use `:StartupTime 500` so we're sure to smooth out any environmental
influence from a spiky system.
