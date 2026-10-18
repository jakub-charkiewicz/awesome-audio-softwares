# Awesome Audio Softwares（日本語）

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

[English README](README.md)

音声処理・音楽制作・可視化・解析に役立つソフトウェアのキュレーションリストです。DAW、エディタ、プラグインホスト、オープンソースツール、ビジュアライゼーション、解析ツールをカバーします。 ⭐ バッジは GitHub のスター数をリアルタイム表示します(shields.io)。

## 目次

- [DAW](#daw)
- [オーディオエディタ](#オーディオエディタ)
- [プラグインホストとフォーマット](#プラグインホストとフォーマット)
- [エフェクト・処理](#エフェクト処理)
- [シンセ・モジュラー](#シンセモジュラー)
- [音楽ビジュアライゼーション](#音楽ビジュアライゼーション)
- [オーディオ解析・メーター](#オーディオ解析メーター)
- [DJ・ライブ](#djライブ)
- [インフラ・I/O](#インフラio)
- [ライブラリ・フレームワーク](#ライブラリフレームワーク)
- [関連リスト](#関連リスト)
- [コントリビューション](#コントリビューション)
- [shvyac の awesome リスト](#shvyac-の-awesome-リスト)

---

## DAW

マルチトラック録音、MIDI、ミキシング、アレンジ向けのデジタル・オーディオ・ワークステーション。

### オープンソース / 無料

- [Ardour](https://ardour.org/) - プロ向けオープンソース DAW。オーディオ/MIDI 録音・ミキシング・オートメーション、プラグインホスト（LV2、VST2/VST3、AU、LADSPA）。Linux / macOS / Windows。現行の 9.x 系でキー/スケール対応を追加。
- [LMMS](https://lmms.io/) - エレクトロニック向けオープンソース DAW。パターンシーケンス、ピアノロール、内蔵シンセ/エフェクト、VST/SoundFont。1.3 系はアルファ版（1.3.0-alpha.2、2026年9月）で安定版に向けて開発中。([GitHub](https://github.com/LMMS/lmms) ![GitHub stars](https://img.shields.io/github/stars/LMMS/lmms?style=flat&label=%E2%AD%90))
- [Qtractor](https://qtractor.sourceforge.io/) - Qt ベースの Linux DAW。MIDI/オーディオ、JACK 親和のルーティング。
- [Zrythm](https://www.zrythm.org/) - タイムライン編集・オートメーション・LV2/VST/CLAP 対応の現代的 GPL DAW。v2（C++/Qt で書き直し）は 2026 年時点でアルファテスト中。
- [Stargate](https://github.com/stargatedaw/stargate) ![GitHub stars](https://img.shields.io/github/stars/stargatedaw/stargate?style=flat&label=%E2%AD%90) - ルーティング行列と内蔵プラグインを備えた軽量クロスプラットフォーム DAW。低スペック向けも意識。
- [openDAW](https://opendaw.studio/) - インストールや登録不要でブラウザ上で動く無料オープンソースの Web DAW。音楽教育向けを重視。AGPL-3.0 と商用ライセンスのデュアルライセンス。([GitHub](https://github.com/andremichelle/openDAW) ![GitHub stars](https://img.shields.io/github/stars/andremichelle/openDAW?style=flat&label=%E2%AD%90))
- [Waveform Free](https://www.tracktion.com/products/waveform-free) - Tracktion Waveform の無料版（現行は Waveform Free 14）。プラグインホスト付きのフル DAW（登録が必要）。
- [Cakewalk Sonar](https://www.cakewalk.com/sonar) - フル機能の Windows DAW。提供終了した Cakewalk by BandLab（旧 SONAR 系）の後継。メンバーシップ不要の無料ティアあり、既存の `.cwp` プロジェクトも開ける。Windows 11 が必要。

### 商用（参考）

広く使われる商用 DAW。相互運用やワークフローの文脈用。

- [REAPER](https://www.reaper.fm/) - 軽量でスクリプト性の高い DAW（Cockos）。幅広いプラグイン形式（VST/VST3/AU/CLAP/LV2/JS）と寛容な評価ライセンス。([cockos.com/reaper](https://www.cockos.com/reaper/))
- [Ableton Live](https://www.ableton.com/live/) - セッション/アレンジ型。エレクトロニックとライブ向けに人気（Live 12）。
- [Logic Pro](https://www.apple.com/logic-pro/) - Apple の macOS/iPad DAW。内蔵音源とミキシングが充実。買い切りのほか、サブスクリプションの Apple Creator Studio バンドルにも含まれる。
- [FL Studio](https://www.image-line.com/fl-studio/) - パターン/プレイリスト中心の DAW（Image-Line）。ビートメイキングに強い。
- [Cubase](https://www.steinberg.net/cubase/) - Steinberg の定番制作 DAW。VST エコシステムの起点。
- [Bitwig Studio](https://www.bitwig.com/) - モジュラー/クリップランチャー型。The Grid と変調・ルーティングが特徴。

---

## オーディオエディタ

録音、クリーンアップ、ポッドキャスト、ファイル編集向け。

- [Audacity](https://www.audacityteam.org/) - 無料オープンソースのマルチトラック音声エディタ/レコーダ。ポッドキャストや簡易編集に定番。VST3/Nyquist。Audacity 4（2026年9月）は Qt ベースで作り直され、非破壊・重ね/グループ化可能なクリップ、UI 刷新、ワークスペース、新プロジェクト形式 `.aup4` を導入。MIDI トラック・ミキサー・マクロは 4.0 では未搭載で、3.7.x 系も引き続き修正版が出ている。([GitHub](https://github.com/audacity/audacity) ![GitHub stars](https://img.shields.io/github/stars/audacity/audacity?style=flat&label=%E2%AD%90)、[変更履歴](https://www.audacityteam.org/changelog/))
- [Tenacity](https://tenacityaudio.org/) - Audacity のコミュニティフォーク。libre 寄りの既定とプラグイン形式（VST、LV2、LADSPA、AU）。開発は Codeberg で行われ GitHub は読み取り専用ミラー。1.3.5（2026年7月）でネイティブ ASIO、Windows on ARM、macOS ビルド復活。([Codeberg](https://codeberg.org/tenacityteam/tenacity))
- [Ocenaudio](https://www.ocenaudio.com/) - リアルタイムエフェクトプレビュー、VST、強力なスペクトログラムを備えた無料クロスプラットフォームエディタ。

---

## プラグインホストとフォーマット

スタンドアロンホストとプラグインが出荷される形式。

- [Carla](https://kx.studio/Applications:Carla) - モジュラー型プラグインホスト（KXStudio）。LADSPA、DSSI、LV2、VST2/VST3、AU、SF2/SFZ。JACK およびネイティブドライバ。([GitHub](https://github.com/falkTX/Carla) ![GitHub stars](https://img.shields.io/github/stars/falkTX/Carla?style=flat&label=%E2%AD%90))
- [LV2](https://lv2plug.in/) - Linux を中心に広く使われるオープンなプラグイン規格（LADSPA/DSSI 系の後継）。
- [CLAP](https://cleveraudio.org/) - 現代的なオープンプラグイン API（CLever Audio Plugin）。ホスト/プラグイン対応が拡大中。
- [JUCE](https://juce.com/) - 多くの商用・OSS オーディオアプリ/プラグインに使われるクロスプラットフォーム C++ フレームワーク。

---

## エフェクト・処理

FX スイート、リスニング向けツール、処理チェーン。

- [LSP Plugins](https://lsp-plug.in/) - EQ・ダイナミクス・メーター・空間系など大規模なオープンソースプロセッサ群（LV2/LADSPA/VST/CLAP およびスタンドアロン）。
- [EffeTune](https://github.com/Frieve-A/effetune) ![GitHub stars](https://img.shields.io/github/stars/Frieve-A/effetune?style=flat&label=%E2%AD%90) - Frieve-A による、音楽鑑賞体験を向上させる無料のリアルタイムオーディオエフェクトプロセッサー。EQ・真空管アンプ・ルーム補正・ビジュアライザーなど 100 種以上のエフェクトを Web/PWA、デスクトップアプリ、Chrome/Edge 拡張、VST3 で提供。
- [Airwindows Consolidated](https://www.airwindows.com/consolidated/) - Chris Johnson による無料・MIT ライセンスの Airwindows エフェクト全種を 1 つにまとめたプラグイン（CLAP/VST3/AU/LV2、macOS/Windows/Linux）。
- [ZL Equalizer](https://zl-audio.github.io/plugins/zlequalizer2/) - 無料オープンソース（AGPL-3.0）のダイナミックイコライザープラグイン（VST3/AU/LV2/AAX、Windows/macOS/Linux）。([GitHub](https://github.com/ZL-Audio/ZLEqualizer) ![GitHub stars](https://img.shields.io/github/stars/ZL-Audio/ZLEqualizer?style=flat&label=%E2%AD%90))
- [Neural Amp Modeler](https://www.neuralampmodeler.com/) - ニューラルネットでギターアンプ/ペダルをキャプチャ・再生する無料オープンソースプラグイン。コミュニティのモデルが豊富。([GitHub](https://github.com/sdatkinson/NeuralAmpModelerPlugin) ![GitHub stars](https://img.shields.io/github/stars/sdatkinson/NeuralAmpModelerPlugin?style=flat&label=%E2%AD%90))
- [Ultimate Vocal Remover](https://github.com/Anjok07/ultimatevocalremovergui) ![GitHub stars](https://img.shields.io/github/stars/Anjok07/ultimatevocalremovergui?style=flat&label=%E2%AD%90) - Demucs や MDX-Net などのモデルを使う AI ステム分離（ボーカル/伴奏/ドラム等）のオープンソース GUI。
- [The Infinite Crate](https://magenta.withgoogle.com/infinite-crate) - Google Magenta による、リアルタイム音楽生成モデル Lyria RealTime を DAW に持ち込み、テキストプロンプトからサンプリング素材を生成できるプラグイン（VST3/AU、macOS/Windows）。2026年3月に Apache-2.0 でオープンソース化。([GitHub](https://github.com/magenta/the-infinite-crate) ![GitHub stars](https://img.shields.io/github/stars/magenta/the-infinite-crate?style=flat&label=%E2%AD%90))
- ホスト内蔵 FX - 上記 DAW の多くは有用な EQ・ダイナミクス・ディレイ・リバーブを同梱。主要チェーンは耐久性のある公式ドキュメントを優先。

---

## シンセ・モジュラー

楽器、モジュラー環境、ドラムマシン。

- [VCV Rack](https://vcvrack.com/) - 仮想 Eurorack モジュラーシンセ。無料の Rack Free と商用モジュール。DAW プラグインあり。
- [Cardinal](https://cardinal.kx.studio/) - VCV Rack 系のオープンソースモジュラー（プラグイン/スタンドアロン）。([GitHub](https://github.com/DISTRHO/Cardinal) ![GitHub stars](https://img.shields.io/github/stars/DISTRHO/Cardinal?style=flat&label=%E2%AD%90))
- [plugdata](https://plugdata.org/) - Pure Data をプラグイン（VST3/AU/LV2/CLAP）およびスタンドアロンで使える、モダンなビジュアルパッチング GUI。([GitHub](https://github.com/plugdata-team/plugdata) ![GitHub stars](https://img.shields.io/github/stars/plugdata-team/plugdata?style=flat&label=%E2%AD%90))
- [Bespoke Synth](https://bespokesynth.com/) - ノードベースのモジュラーシンセ/DAW ハイブリッド。複雑なルーティングと VST ホスト。([GitHub](https://github.com/BespokeSynth/BespokeSynth) ![GitHub stars](https://img.shields.io/github/stars/BespokeSynth/BespokeSynth?style=flat&label=%E2%AD%90))
- [Surge XT](https://surge-synthesizer.github.io/) - オープンソースのハイブリッドシンセ（ウェーブテーブル/FM など）。VST3/AU/LV2/CLAP。([GitHub](https://github.com/surge-synthesizer/surge) ![GitHub stars](https://img.shields.io/github/stars/surge-synthesizer/surge?style=flat&label=%E2%AD%90))
- [OB-Xf](https://github.com/surge-synthesizer/OB-Xf) ![GitHub stars](https://img.shields.io/github/stars/surge-synthesizer/OB-Xf?style=flat&label=%E2%AD%90) - Surge Synth Team による、Oberheim OB-X に着想を得た無料オープンソース（GPL-3.0）のバーチャルアナログシンセ。OB-Xd を現代化した後継。2026 年に安定版 1.0 をリリース（macOS/Windows/Linux）。
- [Dexed](https://asb2m10.github.io/dexed/) - Yamaha DX7 をモデルにしたオープンソース（GPL-3.0）の FM シンセプラグイン（VST/AU/LV2）。DX7 の SysEx カートリッジを読み込み可能。([GitHub](https://github.com/asb2m10/dexed) ![GitHub stars](https://img.shields.io/github/stars/asb2m10/dexed?style=flat&label=%E2%AD%90))
- [OctaSine](https://www.octasine.com/) - FM8 や Elektron Monomachine に着想を得た 4 オペレーターの無料オープンソース（AGPL-3.0、Rust 製）FM シンセ（VST2/CLAP、macOS/Windows/Linux）。最終リリースは v0.9.1（2024年7月）。([GitHub](https://github.com/greatest-ape/OctaSine) ![GitHub stars](https://img.shields.io/github/stars/greatest-ape/OctaSine?style=flat&label=%E2%AD%90))
- [Vital](https://vital.audio/) - スペクトルワーピング型ウェーブテーブルシンセ（無料＋有料ティア）。
- [ZynAddSubFX](https://zynaddsubfx.sourceforge.io/) - 定番オープンソースソフトシンセ（加算/減算/パッド）。([GitHub](https://github.com/zynaddsubfx/zynaddsubfx) ![GitHub stars](https://img.shields.io/github/stars/zynaddsubfx/zynaddsubfx?style=flat&label=%E2%AD%90))
- [Hydrogen](https://github.com/hydrogen-music/hydrogen) ![GitHub stars](https://img.shields.io/github/stars/hydrogen-music/hydrogen?style=flat&label=%E2%AD%90) - オープンソースのドラムマシン/パターンシーケンサ（Linux 中心、他 OS ビルドあり）。

---

## 音楽ビジュアライゼーション

オーディオや MIDI に反応するリアルタイムビジュアル。

- [projectM](https://github.com/projectM-visualizer/projectm) ![GitHub stars](https://img.shields.io/github/stars/projectM-visualizer/projectm?style=flat&label=%E2%AD%90) - MilkDrop 互換のクロスプラットフォーム OSS 音楽ビジュアライゼーションライブラリ。OpenGL でリアルタイム描画。
- [MilkDrop](https://en.wikipedia.org/wiki/MilkDrop) - Ryan Geiss による Winamp 用の定番ハードウェア加速ビジュアライザ。ビート同期のユーザー「プリセット」。
- [Advanced Visualization Studio (AVS)](https://en.wikipedia.org/wiki/Advanced_Visualization_Studio) - Nullsoft による Winamp 用ビジュアライザ。独自エフェクトチェーンを構築可能。
- [G-Force](https://en.wikipedia.org/wiki/G-Force_(visualization_software)) - Andy O'Meara による人気ビジュアライザ。精巧で有機的な 3D ビジュアル。
- [harmony_visualizer](https://github.com/Frieve-A/harmony_visualizer) ![GitHub stars](https://img.shields.io/github/stars/Frieve-A/harmony_visualizer?style=flat&label=%E2%AD%90) - Frieve-A による、MIDI 入力のハーモニー可視化ツール。

---

## オーディオ解析・メーター

スペクトログラム、MIR、ラウドネスメーター、レビュー用ユーティリティ。

- [Sonic Visualiser](https://www.sonicvisualiser.org/) - 音楽録音の詳細な可視化・解析・注釈向けオープンソースアプリ。Vamp フィーチャプラグイン対応。([GitHub](https://github.com/sonic-visualiser/sonic-visualiser) ![GitHub stars](https://img.shields.io/github/stars/sonic-visualiser/sonic-visualiser?style=flat&label=%E2%AD%90))
- [Spek](https://github.com/alexkay/spek) ![GitHub stars](https://img.shields.io/github/stars/alexkay/spek?style=flat&label=%E2%AD%90) - エンコードや転送確認向けの軽量オープンソース音響スペクトル解析（スペクトログラム）。最終リリースは 0.8.5（2023年）。旧ドメイン spek.cc は現在プロジェクトのサイトではない。
- [Prism](https://github.com/Boof2015/prism) ![GitHub stars](https://img.shields.io/github/stars/Boof2015/prism?style=flat&label=%E2%AD%90) - スペクトラム、オシロ、ベクトルスコープ、スペクトログラム、VU、LUFS などを備えた無料 OSS メーター/ビジュアライザ（デスクトップアプリ、VST3/AU/CLAP プラグイン、ターミナル UI）。
- [Vamp plugins](https://vamp-plugins.org/) - Sonic Visualiser などで使う音声特徴抽出プラグイン API/コレクション。
- [librosa](https://librosa.org/) - 音楽・音声解析向け Python ライブラリ（スペクトログラム、MFCC、onset/beat、MIR）。([GitHub](https://github.com/librosa/librosa) ![GitHub stars](https://img.shields.io/github/stars/librosa/librosa?style=flat&label=%E2%AD%90))
- [aubio](https://aubio.org/) - onset・ピッチ・テンポ・ビート・MFCC 向け C/Python ライブラリと CLI。([GitHub](https://github.com/aubio/aubio) ![GitHub stars](https://img.shields.io/github/stars/aubio/aubio?style=flat&label=%E2%AD%90))
- [Frieve's Sound Toolbox](https://github.com/Frieve-A/sound_toolbox) ![GitHub stars](https://img.shields.io/github/stars/Frieve-A/sound_toolbox?style=flat&label=%E2%AD%90) - Frieve-A によるブラウザ上のサウンド関連ツール集。プレビュープレーヤー、ABX テスター、デジタルサンプリングビジュアライザーなど。
- [DIP Bench](https://github.com/Frieve-A/dipbench) ![GitHub stars](https://img.shields.io/github/stars/Frieve-A/dipbench?style=flat&label=%E2%AD%90) - Frieve-A によるデジタルピアノのベンチマークツール。
- [Audio Review](https://github.com/Frieve-A/audioreview) ![GitHub stars](https://img.shields.io/github/stars/Frieve-A/audioreview?style=flat&label=%E2%AD%90) - Frieve-A による、ヘッドフォン・スピーカー・アンプなどを客観評価するレビューサイトのソース。

---

## DJ・ライブ

- [Mixxx](https://mixxx.org/) - ビートマッチ、エフェクト、MIDI/HID コントローラ、ライブラリ管理を備えた無料オープンソース DJ ソフト。([GitHub](https://github.com/mixxxdj/mixxx) ![GitHub stars](https://img.shields.io/github/stars/mixxxdj/mixxx?style=flat&label=%E2%AD%90))

---

## インフラ・I/O

多くの Linux（および一部クロスプラットフォーム）ツールの下で使う低レイテンシ音声配管。

- [JACK](https://jackaudio.org/) - プロ向け低レイテンシ音声接続キット。Linux スタジオグラフの中核として依然重要。
- [PipeWire](https://pipewire.org/) - PulseAudio と JACK を置き換え/橋渡しできる現代的な Linux マルチメディアサーバー。
- [SonoBus](https://sonobus.net/) - リモートセッションや共同作業向けの、低レイテンシ P2P ネットワーク音声ストリーミング（OSS、スタンドアロン/プラグイン）。最終リリースは v1.7.2（2023年12月）。([GitHub](https://github.com/sonosaurus/sonobus) ![GitHub stars](https://img.shields.io/github/stars/sonosaurus/sonobus?style=flat&label=%E2%AD%90))

---

## ライブラリ・フレームワーク

アプリ、プラグイン、研究コードの構成要素。

- [JUCE](https://juce.com/) - [プラグインホストとフォーマット](#プラグインホストとフォーマット) を参照。
- [librosa](https://librosa.org/) / [aubio](https://aubio.org/) - [オーディオ解析・メーター](#オーディオ解析メーター) を参照。

---

## 関連リスト

- [OpenAudio](https://github.com/webprofusion/OpenAudio) ![GitHub stars](https://img.shields.io/github/stars/webprofusion/OpenAudio?style=flat&label=%E2%AD%90) - オープンソースのオーディオアプリ・プラグイン・ライブラリのカタログ。
- [awesome-linuxaudio](https://github.com/nodiscc/awesome-linuxaudio) ![GitHub stars](https://img.shields.io/github/stars/nodiscc/awesome-linuxaudio?style=flat&label=%E2%AD%90) - Linux 向けオーディオソフトの大規模リスト（DAW、シンセ、エフェクト、ユーティリティ）。
- [awesome-audio-dsp](https://github.com/BillyDM/awesome-audio-dsp) ![GitHub stars](https://img.shields.io/github/stars/BillyDM/awesome-audio-dsp?style=flat&label=%E2%AD%90) - オーディオ DSP リソース、OSS プラグイン、学習素材。
- [Linux DAW](https://linuxdaw.org/) - Linux DAW / プラグインのキュレーションディレクトリ。
- [awesome.re](https://awesome.re/) - Awesome マニフェスト。

---

## コントリビューション

コントリビューション歓迎です。ツール追加、リンク切れ修正、カテゴリ提案はプルリクエストでどうぞ。

**公式/ドキュメントの耐久性のある URL**、短い説明、実出荷されているツールを優先してください。製品名はそのまま。オープンソースは明示すると分かりやすいです。

## ライセンス

[LICENSE](LICENSE) を参照してください。

## shvyac の awesome リスト

[shvyac](https://github.com/shvyac) が管理しているキュレーションリストの一覧:

- [awesome-hamradio](https://github.com/shvyac/awesome-hamradio) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-hamradio?style=flat&label=%E2%AD%90)
- [awesome-cad-cae](https://github.com/shvyac/awesome-cad-cae) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-cad-cae?style=flat&label=%E2%AD%90)
- [awesome-map-gis](https://github.com/shvyac/awesome-map-gis) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-map-gis?style=flat&label=%E2%AD%90)
- [awesome-ballroom-dance](https://github.com/shvyac/awesome-ballroom-dance) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-ballroom-dance?style=flat&label=%E2%AD%90)
- [awesome-ghost-artists](https://github.com/shvyac/awesome-ghost-artists) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-ghost-artists?style=flat&label=%E2%AD%90)
- [awesome-audio-softwares](https://github.com/shvyac/awesome-audio-softwares) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-audio-softwares?style=flat&label=%E2%AD%90)
- [awesome-online-services](https://github.com/shvyac/awesome-online-services) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-online-services?style=flat&label=%E2%AD%90)
- [awesome-trading-stock](https://github.com/shvyac/awesome-trading-stock) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-trading-stock?style=flat&label=%E2%AD%90)
- [awesome-open-source-solvers](https://github.com/shvyac/awesome-open-source-solvers) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-open-source-solvers?style=flat&label=%E2%AD%90)
- [awesome-m5stack-arduino](https://github.com/shvyac/awesome-m5stack-arduino) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-m5stack-arduino?style=flat&label=%E2%AD%90)
- [awesome-AI-Powered-Executive-Dashboards](https://github.com/shvyac/awesome-AI-Powered-Executive-Dashboards) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-AI-Powered-Executive-Dashboards?style=flat&label=%E2%AD%90)
- [awesome-ai-tool-for-mechanical-engineering](https://github.com/shvyac/awesome-ai-tool-for-mechanical-engineering) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-ai-tool-for-mechanical-engineering?style=flat&label=%E2%AD%90)
- [awesome-local-llm](https://github.com/shvyac/awesome-local-llm) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-local-llm?style=flat&label=%E2%AD%90)
- [awesome-redmine-ai](https://github.com/shvyac/awesome-redmine-ai) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-redmine-ai?style=flat&label=%E2%AD%90)
- [awesome-dashboards-visualization](https://github.com/shvyac/awesome-dashboards-visualization) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-dashboards-visualization?style=flat&label=%E2%AD%90)
- [awesome-osint-ai](https://github.com/shvyac/awesome-osint-ai) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-osint-ai?style=flat&label=%E2%AD%90)
- [awesome-cms-ai](https://github.com/shvyac/awesome-cms-ai) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-cms-ai?style=flat&label=%E2%AD%90)
