# Awesome Audio Softwares

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

[日本語版はこちら / Japanese](README.ja.md)

A curated list of useful audio software — DAWs, editors, plugin hosts, open-source tools, visualization, and analysis — for musicians, engineers, researchers, and makers. ⭐ badges show live GitHub star counts (via shields.io).

## Contents

- [DAWs](#daws)
- [Audio editors](#audio-editors)
- [Plugin hosts & formats](#plugin-hosts--formats)
- [Effects & processing](#effects--processing)
- [Synthesizers & modular](#synthesizers--modular)
- [Music visualization](#music-visualization)
- [Audio analysis & metering](#audio-analysis--metering)
- [DJ & live](#dj--live)
- [Infrastructure & I/O](#infrastructure--io)
- [Libraries & frameworks](#libraries--frameworks)
- [Related lists](#related-lists)
- [Contributing](#contributing)
- [shvyac's awesome lists](#shvyacs-awesome-lists)

---

## DAWs

Digital audio workstations for multitrack recording, MIDI, mixing, and arranging.

### Open source / free

- [Ardour](https://ardour.org/) - Professional open-source DAW for audio/MIDI recording, mixing, automation, and plugin hosting (LV2, VST2/VST3, AU, LADSPA). Linux, macOS, Windows. Current 9.x series adds keys & scales support.
- [LMMS](https://lmms.io/) - Open-source DAW focused on electronic music: pattern sequencing, piano roll, built-in synths/effects, VST/SoundFont support. The 1.3 series is in alpha (1.3.0-alpha.2, Sep 2026) on the way to a stable release. ([GitHub](https://github.com/LMMS/lmms) ![GitHub stars](https://img.shields.io/github/stars/LMMS/lmms?style=flat&label=%E2%AD%90))
- [Qtractor](https://qtractor.sourceforge.io/) - Qt-based Linux DAW for MIDI and audio with JACK-friendly routing.
- [Zrythm](https://www.zrythm.org/) - Modern GPL DAW with timeline editing, automation, and LV2/VST/CLAP plugin support. v2 (C++/Qt rewrite) is in alpha testing as of 2026.
- [Stargate](https://github.com/stargatedaw/stargate) ![GitHub stars](https://img.shields.io/github/stars/stargatedaw/stargate?style=flat&label=%E2%AD%90) - Lightweight cross-platform DAW with a routing matrix and built-in plugin suite; aims to run well on modest hardware.
- [openDAW](https://opendaw.studio/) - Free, open-source web-based DAW that runs in the browser with no install or sign-up; aimed at music education. AGPL-3.0 with a commercial dual license. ([GitHub](https://github.com/andremichelle/openDAW) ![GitHub stars](https://img.shields.io/github/stars/andremichelle/openDAW?style=flat&label=%E2%AD%90))
- [Waveform Free](https://www.tracktion.com/products/waveform-free) - Free edition of Tracktion Waveform (currently Waveform Free 14); full DAW feature set with plugin hosting (registration required).
- [Cakewalk Sonar](https://www.cakewalk.com/sonar) - Full-featured Windows DAW; successor to the now-retired Cakewalk by BandLab (formerly SONAR). Free tier usable without a membership; opens existing `.cwp` projects. Requires Windows 11.

### Commercial (reference)

Widely used commercial DAWs; listed for interoperability and workflow context.

- [REAPER](https://www.reaper.fm/) - Efficient, highly scriptable DAW (Cockos) with broad plugin format support (VST/VST3/AU/CLAP/LV2/JS) and a generous evaluation license. ([cockos.com/reaper](https://www.cockos.com/reaper/))
- [Ableton Live](https://www.ableton.com/live/) - Session/arrangement DAW popular for electronic music and live performance (Live 12).
- [Logic Pro](https://www.apple.com/logic-pro/) - Apple's macOS/iPad DAW with deep stock instruments and mixing tools. Sold as a one-time purchase or as part of the Apple Creator Studio subscription bundle.
- [FL Studio](https://www.image-line.com/fl-studio/) - Pattern- and playlist-oriented DAW (Image-Line) with strong beat-making workflows.
- [Cubase](https://www.steinberg.net/cubase/) - Steinberg's long-running production DAW; origin of the VST ecosystem.
- [Bitwig Studio](https://www.bitwig.com/) - Modular, clip-launcher DAW with The Grid and strong modulation/routing.

---

## Audio editors

Multitrack or destructive editors for recording, cleanup, podcasts, and file work.

- [Audacity](https://www.audacityteam.org/) - Free, open-source multitrack audio editor and recorder; widely used for podcasts, cleanup, and simple editing. VST3/Nyquist plugins. Audacity 4 (Sep 2026) is rebuilt on Qt with non-destructive, overlapping/groupable clips, a redesigned UI, workspaces, and a new `.aup4` project format; MIDI tracks, the Mixer, and Macros are not yet in 4.0, and the 3.7.x line still receives fixes. ([GitHub](https://github.com/audacity/audacity) ![GitHub stars](https://img.shields.io/github/stars/audacity/audacity?style=flat&label=%E2%AD%90), [Changelog](https://www.audacityteam.org/changelog/))
- [Tenacity](https://tenacityaudio.org/) - Community fork of Audacity focused on libre defaults and plugin formats (VST, LV2, LADSPA, AU). Developed on Codeberg (GitHub is a read-only mirror); 1.3.5 (Jul 2026) adds native ASIO, Windows on ARM, and restored macOS builds. ([Codeberg](https://codeberg.org/tenacityteam/tenacity))
- [Ocenaudio](https://www.ocenaudio.com/) - Free cross-platform audio editor with real-time effects preview, VST support, and a strong spectrogram view.

---

## Plugin hosts & formats

Standalone hosts and the formats plugins ship in.

- [Carla](https://kx.studio/Applications:Carla) - Modular plugin host (KXStudio): LADSPA, DSSI, LV2, VST2/VST3, AU, SF2/SFZ; JACK and native drivers. ([GitHub](https://github.com/falkTX/Carla) ![GitHub stars](https://img.shields.io/github/stars/falkTX/Carla?style=flat&label=%E2%AD%90))
- [LV2](https://lv2plug.in/) - Open plugin standard widely used on Linux (and elsewhere); successor lineage to LADSPA/DSSI.
- [CLAP](https://cleveraudio.org/) - Modern open plugin API (CLever Audio Plugin) with growing host/plugin support.
- [JUCE](https://juce.com/) - Cross-platform C++ framework used to build many commercial and open-source audio apps and plugins.

---

## Effects & processing

FX suites, listening tools, and processing chains.

- [LSP Plugins](https://lsp-plug.in/) - Large open-source suite of studio processors (EQ, dynamics, metering, spatial, etc.) in LV2/LADSPA/VST/CLAP and standalone forms.
- [EffeTune](https://github.com/Frieve-A/effetune) ![GitHub stars](https://img.shields.io/github/stars/Frieve-A/effetune?style=flat&label=%E2%AD%90) - Free real-time audio effect processor by Frieve-A for enhancing music listening: 100+ effects (EQ, tube amp, room correction, visualizers, etc.) as a Web/PWA, desktop app, Chrome/Edge extension, and VST3.
- [Airwindows Consolidated](https://www.airwindows.com/consolidated/) - All of Chris Johnson's free, MIT-licensed Airwindows effects in a single plugin (CLAP/VST3/AU/LV2) for macOS, Windows, and Linux.
- [ZL Equalizer](https://zl-audio.github.io/plugins/zlequalizer2/) - Free, open-source (AGPL-3.0) dynamic equalizer plugin (VST3/AU/LV2/AAX) for Windows, macOS, and Linux. ([GitHub](https://github.com/ZL-Audio/ZLEqualizer) ![GitHub stars](https://img.shields.io/github/stars/ZL-Audio/ZLEqualizer?style=flat&label=%E2%AD%90))
- [Neural Amp Modeler](https://www.neuralampmodeler.com/) - Free, open-source neural-network guitar amp/pedal capture and playback plugin; large community model library. ([GitHub](https://github.com/sdatkinson/NeuralAmpModelerPlugin) ![GitHub stars](https://img.shields.io/github/stars/sdatkinson/NeuralAmpModelerPlugin?style=flat&label=%E2%AD%90))
- [Ultimate Vocal Remover](https://github.com/Anjok07/ultimatevocalremovergui) ![GitHub stars](https://img.shields.io/github/stars/Anjok07/ultimatevocalremovergui?style=flat&label=%E2%AD%90) - Open-source GUI for AI stem separation (vocals/instrumental/drums, etc.) using Demucs, MDX-Net, and other models.
- [The Infinite Crate](https://magenta.withgoogle.com/infinite-crate) - Google Magenta's DAW plugin (VST3/AU) for macOS and Windows that brings the Lyria RealTime live music model into the DAW, generating music from text prompts for sampling; open-sourced under Apache-2.0 in Mar 2026. ([GitHub](https://github.com/magenta/the-infinite-crate) ![GitHub stars](https://img.shields.io/github/stars/magenta/the-infinite-crate?style=flat&label=%E2%AD%90))
- Stock / host FX - Most DAWs above ship useful EQ, dynamics, delay, and reverb; prefer durable host docs when choosing a primary chain.

---

## Synthesizers & modular

Instruments, modular environments, and drum machines.

- [VCV Rack](https://vcvrack.com/) - Virtual Eurorack modular synthesizer; free Rack Free edition plus commercial modules; DAW plugins available.
- [Cardinal](https://cardinal.kx.studio/) - Open-source modular synthesizer / VCV Rack fork as plugin and standalone. ([GitHub](https://github.com/DISTRHO/Cardinal) ![GitHub stars](https://img.shields.io/github/stars/DISTRHO/Cardinal?style=flat&label=%E2%AD%90))
- [plugdata](https://plugdata.org/) - Pure Data as a plugin (VST3/AU/LV2/CLAP) and standalone app with a modern visual patching GUI. ([GitHub](https://github.com/plugdata-team/plugdata) ![GitHub stars](https://img.shields.io/github/stars/plugdata-team/plugdata?style=flat&label=%E2%AD%90))
- [Bespoke Synth](https://bespokesynth.com/) - Modular node-based synth/DAW hybrid with complex routing and VST hosting. ([GitHub](https://github.com/BespokeSynth/BespokeSynth) ![GitHub stars](https://img.shields.io/github/stars/BespokeSynth/BespokeSynth?style=flat&label=%E2%AD%90))
- [Surge XT](https://surge-synthesizer.github.io/) - Open-source hybrid synthesizer (wavetable / FM / etc.) as VST3/AU/LV2/CLAP. ([GitHub](https://github.com/surge-synthesizer/surge) ![GitHub stars](https://img.shields.io/github/stars/surge-synthesizer/surge?style=flat&label=%E2%AD%90))
- [OB-Xf](https://github.com/surge-synthesizer/OB-Xf) ![GitHub stars](https://img.shields.io/github/stars/surge-synthesizer/OB-Xf?style=flat&label=%E2%AD%90) - Free, open-source (GPL-3.0) Oberheim OB-X-inspired virtual analog synth from the Surge Synth Team; a modernized continuation of OB-Xd. Stable 1.0 released in 2026 for macOS, Windows, and Linux.
- [Dexed](https://asb2m10.github.io/dexed/) - Open-source (GPL-3.0) FM synthesizer modeled on the Yamaha DX7 (VST/AU/LV2); loads DX7 SysEx cartridges. ([GitHub](https://github.com/asb2m10/dexed) ![GitHub stars](https://img.shields.io/github/stars/asb2m10/dexed?style=flat&label=%E2%AD%90))
- [OctaSine](https://www.octasine.com/) - Free, open-source (AGPL-3.0, Rust) four-operator FM synthesizer inspired by FM8 and the Elektron Monomachine (VST2/CLAP; macOS, Windows, Linux). Last release v0.9.1 (Jul 2024). ([GitHub](https://github.com/greatest-ape/OctaSine) ![GitHub stars](https://img.shields.io/github/stars/greatest-ape/OctaSine?style=flat&label=%E2%AD%90))
- [Vital](https://vital.audio/) - Spectral warping wavetable synthesizer (free + paid tiers).
- [ZynAddSubFX](https://zynaddsubfx.sourceforge.io/) - Classic open-source softsynth (additive / subtractive / pad). ([GitHub](https://github.com/zynaddsubfx/zynaddsubfx) ![GitHub stars](https://img.shields.io/github/stars/zynaddsubfx/zynaddsubfx?style=flat&label=%E2%AD%90))
- [Hydrogen](https://github.com/hydrogen-music/hydrogen) ![GitHub stars](https://img.shields.io/github/stars/hydrogen-music/hydrogen?style=flat&label=%E2%AD%90) - Open-source drum machine / pattern sequencer (Linux-focused; cross-builds available).

---

## Music visualization

Real-time visuals driven by audio or MIDI.

- [projectM](https://github.com/projectM-visualizer/projectm) ![GitHub stars](https://img.shields.io/github/stars/projectM-visualizer/projectm?style=flat&label=%E2%AD%90) - Cross-platform, open-source music visualization library that is MilkDrop-compatible, rendering real-time audio-reactive visuals via OpenGL.
- [MilkDrop](https://www.geisswerks.com/milkdrop/) - Classic hardware-accelerated music visualization plugin for Winamp by Ryan Geiss; beat-synced user "presets."
- [Advanced Visualization Studio (AVS)](https://github.com/visbot/vis_avs) ![GitHub stars](https://img.shields.io/github/stars/visbot/vis_avs?style=flat&label=%E2%AD%90) - Winamp visualization plugin by Nullsoft for building custom visual effect chains (open-sourced AVS 2.81d code).
- [G-Force](https://www.soundspectrum.com/g-force/) - Music visualization plugin by Andy O'Meara (SoundSpectrum) known for detailed, organic 3D visuals.
- [harmony_visualizer](https://github.com/Frieve-A/harmony_visualizer) ![GitHub stars](https://img.shields.io/github/stars/Frieve-A/harmony_visualizer?style=flat&label=%E2%AD%90) - Tool by Frieve-A for visualizing the harmony of MIDI input.

---

## Audio analysis & metering

Spectrograms, MIR tools, loudness meters, and review utilities.

- [Sonic Visualiser](https://www.sonicvisualiser.org/) - Open-source app for detailed visualization, analysis, and annotation of music recordings; Vamp feature plugins. ([GitHub](https://github.com/sonic-visualiser/sonic-visualiser) ![GitHub stars](https://img.shields.io/github/stars/sonic-visualiser/sonic-visualiser?style=flat&label=%E2%AD%90))
- [Spek](https://github.com/alexkay/spek) ![GitHub stars](https://img.shields.io/github/stars/alexkay/spek?style=flat&label=%E2%AD%90) - Lightweight open-source acoustic spectrum analyser (spectrogram) for checking encodes and transfers. Last release 0.8.5 (2023); the former spek.cc domain no longer hosts the project.
- [Prism](https://github.com/Boof2015/prism) ![GitHub stars](https://img.shields.io/github/stars/Boof2015/prism?style=flat&label=%E2%AD%90) - Free open-source meter/visualizer rack (spectrum, scope, vectorscope, spectrogram, VU, LUFS) as a desktop app, VST3/AU/CLAP plugins, and a terminal UI.
- [Vamp plugins](https://vamp-plugins.org/) - Plugin API and collection for audio feature extraction used by Sonic Visualiser and related tools.
- [librosa](https://librosa.org/) - Python library for music and audio analysis (spectrograms, MFCCs, onset/beat, MIR pipelines). ([GitHub](https://github.com/librosa/librosa) ![GitHub stars](https://img.shields.io/github/stars/librosa/librosa?style=flat&label=%E2%AD%90))
- [aubio](https://aubio.org/) - C/Python library and CLI tools for onset, pitch, tempo, beat, and MFCC analysis. ([GitHub](https://github.com/aubio/aubio) ![GitHub stars](https://img.shields.io/github/stars/aubio/aubio?style=flat&label=%E2%AD%90))
- [Frieve's Sound Toolbox](https://github.com/Frieve-A/sound_toolbox) ![GitHub stars](https://img.shields.io/github/stars/Frieve-A/sound_toolbox?style=flat&label=%E2%AD%90) - Browser-based sound tools by Frieve-A: preview player, ABX tester, digital sampling visualizer, and more.
- [DIP Bench](https://github.com/Frieve-A/dipbench) ![GitHub stars](https://img.shields.io/github/stars/Frieve-A/dipbench?style=flat&label=%E2%AD%90) - Digital piano benchmark tool by Frieve-A.
- [Audio Review](https://github.com/Frieve-A/audioreview) ![GitHub stars](https://img.shields.io/github/stars/Frieve-A/audioreview?style=flat&label=%E2%AD%90) - Source for an audio equipment review site by Frieve-A with objective evaluations of headphones, speakers, and amplifiers.
- [ABX Blind Test](https://theaudiostuff.com/tools/abx-test/) - Browser-based ABX tester with built-in test pairs or two files of your own, level matching and a fixed round count; runs locally, no upload.

---

## DJ & live

- [Mixxx](https://mixxx.org/) - Free, open-source DJ software with beatmatching, effects, MIDI/HID controllers, and library management. ([GitHub](https://github.com/mixxxdj/mixxx) ![GitHub stars](https://img.shields.io/github/stars/mixxxdj/mixxx?style=flat&label=%E2%AD%90))

---

## Infrastructure & I/O

Low-latency audio plumbing used under many Linux (and some cross-platform) tools.

- [JACK](https://jackaudio.org/) - Professional low-latency audio connection kit; still central to many Linux studio graphs.
- [PipeWire](https://pipewire.org/) - Modern Linux multimedia server that can replace/bridge PulseAudio and JACK for apps and pro-audio graphs.
- [SonoBus](https://sonobus.net/) - Open-source, low-latency peer-to-peer network audio streaming for remote jamming and collaboration; standalone and plugin. Last release v1.7.2 (Dec 2023). ([GitHub](https://github.com/sonosaurus/sonobus) ![GitHub stars](https://img.shields.io/github/stars/sonosaurus/sonobus?style=flat&label=%E2%AD%90))

---

## Libraries & frameworks

Building blocks for apps, plugins, and research code.

- [JUCE](https://juce.com/) - See [Plugin hosts & formats](#plugin-hosts--formats).
- [librosa](https://librosa.org/) / [aubio](https://aubio.org/) - See [Audio analysis & metering](#audio-analysis--metering).

---

## Related lists

- [OpenAudio](https://github.com/webprofusion/OpenAudio) ![GitHub stars](https://img.shields.io/github/stars/webprofusion/OpenAudio?style=flat&label=%E2%AD%90) - Catalog of open-source audio apps, plugins, and libraries.
- [awesome-linuxaudio](https://github.com/nodiscc/awesome-linuxaudio) ![GitHub stars](https://img.shields.io/github/stars/nodiscc/awesome-linuxaudio?style=flat&label=%E2%AD%90) - Extensive Linux audio software list (DAWs, synths, effects, utilities).
- [awesome-audio-dsp](https://github.com/BillyDM/awesome-audio-dsp) ![GitHub stars](https://img.shields.io/github/stars/BillyDM/awesome-audio-dsp?style=flat&label=%E2%AD%90) - Audio DSP resources, open-source plugins, and learning material.
- [Linux DAW](https://linuxdaw.org/) - Curated Linux DAW / plugin directory.
- [awesome.re](https://awesome.re/) - Awesome manifesto.

---

## Contributing

Contributions welcome — open a pull request to add a tool, fix a broken link, or suggest a category.

Prefer **durable official / docs URLs**, short blurbs, and tools that are shipping. Keep product names; mark open-source clearly when helpful.

## License

See [LICENSE](LICENSE).

## shvyac's awesome lists

All curated lists maintained by [shvyac](https://github.com/shvyac):

- [awesome-AI-Powered-Executive-Dashboards](https://github.com/shvyac/awesome-AI-Powered-Executive-Dashboards) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-AI-Powered-Executive-Dashboards?style=flat&label=%E2%AD%90)
- [awesome-ai-tool-for-mechanical-engineering](https://github.com/shvyac/awesome-ai-tool-for-mechanical-engineering) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-ai-tool-for-mechanical-engineering?style=flat&label=%E2%AD%90)
- [awesome-audio-softwares](https://github.com/shvyac/awesome-audio-softwares) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-audio-softwares?style=flat&label=%E2%AD%90)
- [awesome-azure-ai-dynamics365-security](https://github.com/shvyac/awesome-azure-ai-dynamics365-security) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-azure-ai-dynamics365-security?style=flat&label=%E2%AD%90)
- [awesome-ballroom-dance](https://github.com/shvyac/awesome-ballroom-dance) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-ballroom-dance?style=flat&label=%E2%AD%90)
- [awesome-cad-cae](https://github.com/shvyac/awesome-cad-cae) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-cad-cae?style=flat&label=%E2%AD%90)
- [awesome-cms-ai](https://github.com/shvyac/awesome-cms-ai) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-cms-ai?style=flat&label=%E2%AD%90)
- [awesome-dashboards-visualization](https://github.com/shvyac/awesome-dashboards-visualization) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-dashboards-visualization?style=flat&label=%E2%AD%90)
- [awesome-ghost-artists](https://github.com/shvyac/awesome-ghost-artists) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-ghost-artists?style=flat&label=%E2%AD%90)
- [awesome-hamradio](https://github.com/shvyac/awesome-hamradio) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-hamradio?style=flat&label=%E2%AD%90)
- [awesome-hpc](https://github.com/shvyac/awesome-hpc) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-hpc?style=flat&label=%E2%AD%90)
- [awesome-iso27001-isms-tools](https://github.com/shvyac/awesome-iso27001-isms-tools) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-iso27001-isms-tools?style=flat&label=%E2%AD%90)
- [awesome-local-llm](https://github.com/shvyac/awesome-local-llm) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-local-llm?style=flat&label=%E2%AD%90)
- [awesome-m5stack-arduino](https://github.com/shvyac/awesome-m5stack-arduino) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-m5stack-arduino?style=flat&label=%E2%AD%90)
- [awesome-map-gis](https://github.com/shvyac/awesome-map-gis) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-map-gis?style=flat&label=%E2%AD%90)
- [awesome-meshless-cae](https://github.com/shvyac/awesome-meshless-cae) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-meshless-cae?style=flat&label=%E2%AD%90)
- [awesome-online-services](https://github.com/shvyac/awesome-online-services) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-online-services?style=flat&label=%E2%AD%90)
- [awesome-open-source-solvers](https://github.com/shvyac/awesome-open-source-solvers) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-open-source-solvers?style=flat&label=%E2%AD%90)
- [awesome-osint-ai](https://github.com/shvyac/awesome-osint-ai) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-osint-ai?style=flat&label=%E2%AD%90)
- [awesome-redmine-ai](https://github.com/shvyac/awesome-redmine-ai) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-redmine-ai?style=flat&label=%E2%AD%90)
- [awesome-requirements-system-ai](https://github.com/shvyac/awesome-requirements-system-ai) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-requirements-system-ai?style=flat&label=%E2%AD%90)
- [awesome-trading-stock](https://github.com/shvyac/awesome-trading-stock) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-trading-stock?style=flat&label=%E2%AD%90)
