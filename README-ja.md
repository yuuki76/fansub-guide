* __注__: この文書は翻訳版です。リンク切れや追加の提案は [オリジナルの著者](//yukisubs.wordpress.com/about) に。翻訳ミスと思われるものは私にご連絡ください。
* 最終更新: 2020-09-28, 翻訳: 2021-04-06
* [オリジナル](https://yukisubs.wordpress.com/guides) [オリジナルのMarkdown](//gist.github.com/YukinoAi/acea024631a2585aa592b16b4bde959f)
* この記事には著作権違反になる内容が多く含まれていると予想されますが、技術的な価値が非常に高いと考えられるためそれらの内容を除去せず掲載します。この記事の内容を実行する際には個々人の責任でよく考え、自国の法律に抵触しない範囲で実行することをおすすめします。
* リンク先は英語ですが自分で翻訳しろ❓

#### __目次__:

* [ファンサブとは何か](#ファンサブとは何か)
* [キャッピング](#キャッピング)
* [エンコード](#エンコード)
  * 音声
  * 再生 (パソコン/ホームシアターPC)
* [多重化と分割](#多重化と分割)
* [フィルター](#フィルター)
  * シーンフィルター
* [翻訳](#翻訳と検証)
* [編集とチェック](#編集とチェック)
* [字幕タイミング](#字幕タイミング)
* [字幕組版](#字幕組版)
* [配布](#配布)
  * Torrents
  * HTTP/S
  * IRC
  * [便利ツール](#便利ツール)
  * [グループ](#グループ)
  * [配布をDIYするためのガイド](#配布をDIYするためのガイド)
* [再多重化(既存リリースをまとめる)](#最多重化)
* [アナログ](#アナログ処理)

#### __ファンサブとは何か__

* __理論__: [WikiEN:ファンサブの歴史](//en.wikipedia.org/wiki/Fansub) and [ファンサブの現状(死んでる)](http://www.crymore.net/2015/05/15/the-state-of-fansubbing-its-dead).  
  **訳注**: 外国の映像作品を独自に翻訳するボランティア的な試み。ほとんどのリリースが著作権法を無視していることに注意。

* __類似のガイド__:  
  
  訳注:他のファンサブグループが作ってるガイド。
  
  * Doki's [Fansubbing Process Overview](//doki.co/support/the-fansubbing-process), [Portable Document Format (PDF)](//yukisubs.files.wordpress.com/2016/10/the_fansubbing_process_doki_fansubs.pdf).
  * unanimated's [Guide Index](//unanimated.github.io/guides.htm)
    * Typesetting [Guide](//unanimated.github.io/ts/index.htm), [PDF-White](//yukisubs.files.wordpress.com/2020/04/typesetting_in_aegisub_by_unanimated_2018_white.pdf), [PDF-Black](//yukisubs.files.wordpress.com/2020/04/typesetting_in_aegisub_by_unanimated_2018_black.pdf),  [PDF-old](//yukisubs.files.wordpress.com/2016/10/unanimated_fansub_guides.pdf).*(黒と白は単に色の違い)*
  * SubsByRock [Index](//subsbyrock.wordpress.com/links).
  * tekeremata's [whatever this is](http://tekeremata.org/category/articulos/taller-de-fansub/) (Spanish, scroll down).
  * And this random [Idiot's Guide](//fansubbing.blogspot.com/2007/03/what-goes-into-fansub-aka-idiots-guide_05.html).

* [Aegisub](http://docs.aegisub.org/manual/Overview): ファンサブ(字幕作成)のコアツール [配布先](http://plorkyeran.com/aegisub). 
  
  * Aegisubの [マニュアル](http://docs.aegisub.org/manual/Overview), [PDF](//yukisubs.files.wordpress.com/2017/05/aegisub-3-2-manual.pdf), [パス記法](http://docs.aegisub.org/3.2/Aegisub_path_specifiers/) [ASS Override Tags](http://docs.aegisub.org/manual/ASS_Tags).

* [雑多なファンサブに関するガイド](http://mod16.org/hurfdurf/?p=128)

* ファンサブの歴史: [ブログ記事](http://mod16.org/hurfdurf/?p=144), [インタビュー](//uniquec.shinsen-radio.org), [YouTubeプレイリスト](//www.youtube.com/playlist?list=PLtwIkfU56fRSZgaPHFt79ei1_Kf4cDaFY) アーカイブで見る昔のファンサブ: `web.archive.org/web/20021013081748/http://pepper.idge.net:80/digisub.html`, [PDF](//yukisubs.files.wordpress.com/2018/02/digisub_guide_onceuponatimein2002.pdf).

#### __キャッピング__

* __概要__: 作品そのものを手に入れること。
* 最適なのはDVDやBDの無加工(BDMVなど)だが、アップロードされているとは限らない。
* アップロードされていないならメディアの購入から。ファンサブをサポートするために購入を検討する。できないのならば既存のVHS/LD/DVD/BDもしくはWebからのリップで許容できる品質のものを選ぶ。
* リアルタイム放送ならキャッピングは録画すること。特殊なハードで放送自体を録画する。 インターネット[サイマル放送](https://ja.wikipedia.org/wiki/%E3%82%B5%E3%82%A4%E3%83%9E%E3%83%AB%E6%94%BE%E9%80%81) が利用できるなら特別なソフトによって[ストリームコピー](//ffmpeg.org/ffmpeg.html#Stream-copy)することができる。招待制のトラッカーで先述の無加工コピーが手に入ることもある。  
  字幕の抽出に関しては**最多重化**の項を参照。
* アナログテレビ,8mm,VHS,LDに関しては __アナログ__の項を参照。
* __デジタルテレビ,ケーブルテレビ,衛星放送__:  デジタル[信号処理](http://slideplayer.com/slide/6002959/)が参考になる
* __DVD__: [DVD-Decrypter](http://fileforum.betanews.com/detail/DVD-Decrypter/1011845169/1)とそのガイド[DVD Decrypter Guide](http://www.doom9.org/index.html?/dvddec.htm), [PDF版](//yukisubs.files.wordpress.com/2016/10/dvd-decrypter_guide.pdf) [もう一つのガイド](//www.dvd-guides.com/guides/copydvdtodvd/22-how-to-copy-a-dvd-59-using-dvd-decrypter).
* __DVDとBD__: [MakeMKV](//www.makemkv.com), と [HandbrakeとMakeMKVのガイド](//lifehacker.com/5559007/the-hassle-free-guide-to-ripping-your-blu-ray-collection).
* 単なる動画の抽出: [MKVToolNix](//mkvtoolnix.download/downloads.html) + [gMKVExtractGUI](//sourceforge.net/projects/gmkvextractgui), もしくは [FFMPEG](//wiki.archlinux.org/index.php/FFmpeg#Subtitles)。 __最多重化__ も参照
* 字幕の変換: [Subtitle Edit](http://www.nikse.dk/subtitleedit) とその [ドキュメント](http://www.nikse.dk/SubtitleEdit/Help).
* 字幕の抽出には __多重化__ と __最多重化__ の項も参照
* __ウェブ経由のダウンロード:__
  * [youtube-dl](//github.com/rg3/youtube-dl), [GUI版](//github.com/MrS0m30n3/youtube-dl-gui). "業界標準"でCrunchyrollを含む多数のサイトに対応。
    * YouTubeの地域ベースブロックには [地域チェッカー](//unblockvideos.com/youtube-video-restriction-checker) と [VPN](//en.wikipedia.org/wiki/Virtual_private_network) でブロックされていない国に偽装することで対応。
  * *[Crunchyroll-XML-Decoder](//github.com/jaw20/crunchy-xml-decoder) + [workaround instructions](//gist.github.com/gdiaz384/ba8dfc45a44f92840aaf2617f802351f) (January 2017). Supports multilingual subtitle only downloads.*
  * *Crunchyroll Downloader Toolkit DX, [Mediafire](//www.mediafire.com/file/0jevs7wnhh0x0u6/Crunchyroll+Downloader+Toolkit+DX.zip), [Mega](//mega.nz/#F!wUYwDSgA!8tx_37HUBcs9KqPhkk5FmQ).  Windows only. Note: I have not tested this.*
  * *[Crunchyroll-Download-Tool](//gitlab.com/RIP/Crunchyroll-Download-Tool) (extension of DX toolkit for bulk downloads). Note: I have not tested this.*
    * *Seiya's [Funimation-Downloader-nx](//github.com/seiya-dev/funimation-downloader-nx) and [GUI](//github.com/Golumpa/FuniBatchGUI). Note: I have not tested this. Also: related [cat](//yukisubs.files.wordpress.com/2018/02/golumpascat.jpg).* 
    * ネットフリックスだとかアマゾンだとかの配信を録画するには [OBS](//obsproject.com) みたいな画面録画か、手動によるRTMPトランスポートを用いたリッピングぐらいしかない。
      * *Further reading: [netflix-subtitle-downloader](//greasyfork.org/en/scripts/26654-netflix-subtitle-downloader). Note: I have not tested this.*
* DVDやBDMVの無加工、ウェブ経由のDLは他の人から直接入手できるかもしれない。配布セクションを参照。

#### __エンコード__

* __ビデオ理論(基礎)__: 映像は高速で移り変わる画像として説明できる。
* エンコードする理由は、*複雑な変更を(フィルタリングなど)保持し*(訳疑問) ファイルサイズを小さくすること。非圧縮ビデオは1分でも数GBに達する。基本的には目で見た品質をそのままにファイルサイズを"許容可能な"レベルまで落とすこと。
* MPEGは一つの画像(キーフレーム)を圧縮して、そのフレームと次のフレームの差分を取ることを繰り返して動画全体を圧縮する。ゆえに特定のフレームを表示するにはその前のフレームをすべてではないにしろデコードしなければならない
* __ビデオ理論(完全)__: 理論を理解せずエンコードすること良いことではない(問題の原因だ)が、必要となる背景知識が多すぎるため網羅的・体系的に学ぶのは難しい。これは理想に近い:[A&E's Technical Guides to All Things Audio and Video (v3)](//www.animemusicvideos.org/guides/avtech31)__, [PDF](//yukisubs.files.wordpress.com/2016/10/aandes_technical_guides_to_all_things_audio_and_video.pdf). これを全部読め！. __近道はない__. A&E'のガイドは古いが理論を学ぶには問題ない。最新のガイドは以下にある。
* __コーデック,コンテナ理論__:
  * この動画みろ: [How Codecs Work - Tutorial](//vimeo.com/104554788) 
  * コンテナとコーデック: [Media Formats](//www.dr-lex.be/info-stuff/mediaformats.html) and [How to Choose the Right Codec](//www.videomaker.com/article/c03/18165-how-to-choose-the-right-codec-and-container-for-your-video-workflow) and [read this discussion](//collectr.blogspot.com/2011/08/encoding-wars-return-of-revenge-of.html).
  * Wikipedia (Wiki): [Codec Comparison(EN)](//en.wikipedia.org/wiki/Comparison_of_video_codecs), [Container Comparison(EN)](//en.wikipedia.org/wiki/Comparison_of_video_container_formats), [MPEG standards(JP)](https://ja.wikipedia.org/wiki/Moving_Picture_Experts_Group).
  * HEVCレビュー [1](//forums.bakabt.me/index.php?topic=45462.0), [2](//x265.ru/en/bolshoe-sravnenie-kodekov-h265-ot-mgu), [PDF](//yukisubs.files.wordpress.com/2016/10/msu_hevc_comparison_2015_free.pdf) [3](//blogs.gnome.org/rbultje/2015/09/28/vp9-encodingdecoding-performance-vs-hevch-264).
    * 興味深い [ブログ記事](http://archimago.blogspot.com/2016/12/musings-end-of-2016-video-encoding-hevc.html).
    * Kokominiの [x265とOpus/AAC向けエンコーディングガイド](https://kokomins.wordpress.com/2019/10/10/anime-encoding-guide-for-x265-and-why-to-never-use-flac/).
  * 参考: [Video Codecs by FOURCC](https://www.fourcc.org/codecs.php) and [要約](//docs.microsoft.com/en-us/windows/desktop/medfound/video-fourccs).
* __輝度と色彩の理論__:
  * 人間の[色覚](//www.cambridgeincolour.com/tutorials/color-perception.htm) と [特性](//www.cambridgeincolour.com/tutorials/cameras-vs-human-eye.htm).
    * 私達の目はガバガバ: [human blind spot test](https://yukisubs.files.wordpress.com/2020/04/blind-spot-test.jpg).
  * ~~Adobe Video Road blog: [色を理解する](//blogs.adobe.com/VideoRoad/2010/06/understanding_color_processing.html), [YUVとはなにか](//blogs.adobe.com/VideoRoad/2010/06/what_is_yuv.html), [Color Subsampling](//blogs.adobe.com/VideoRoad/2010/06/color_subsampling_or_what_is_4.html).~~ リンク切れ
  * [8-bit と 16-bit](//www.diyphotography.net/8-bit-vs-16-bit-color-depth-use-matters).
  * [色深度チュートリアル](//www.cambridgeincolour.com/tutorials/bit-depth.htm).
  * [Doki - Discussion: 10-bit h264](//doki.co/2011/07/19/discussion-10-bit-h264) PDF版: [10-bit AVC Broadcasting](//yukisubs.files.wordpress.com/2016/10/using_10-bit_avc-h-264_encoding_with_422_for_broadcast_contribution_-_pierre_larbier.pdf), [Why 10-bit Saves Bandwidth](//yukisubs.files.wordpress.com/2016/10/why_does_10bit_save_bandwidth_-_ateme.pdf), [10-bit Presentation](//yukisubs.files.wordpress.com/2016/10/10-bit_pristine_video_quality_presentation_-_ateme.pdf).
    * 関連する [ブログ記事](http://archimago.blogspot.com/2016/12/quick-compare-avc-vs-hevc-8-bit-vs-10.html).
  * [ヒストグラムについて](//www.cambridgeincolour.com/tutorials/histograms1.htm), [Part 2](//www.cambridgeincolour.com/tutorials/histograms2.htm) と [実例](//yukisubs.files.wordpress.com/2018/06/beluga.jpg).
  * [ホワイトバランスとは](//www.cambridgeincolour.com/tutorials/white-balance.htm).
  * [ダイナミックレンジとは](//www.cambridgeincolour.com/tutorials/dynamic-range.htm).
  * 興味深い実例:
    * Wiki: [色空間](https://ja.wikipedia.org/wiki/%E8%89%B2%E7%A9%BA%E9%96%93), [Rec601](//en.wikipedia.org/wiki/Rec._601) と [Rec709](//en.wikipedia.org/wiki/Rec._709).
    * [NTSCとPALの原色について](//video.stackexchange.com/questions/16840/ffmpeg-explicitly-tag-h-264-as-bt-601-rather-than-leaving-unspecified).
    * [YCbCrのデータ範囲の例](http://discoverybiz.net/enu0/faq/faq_YUVDataRangeByBreeze.html).
    * [YUV サブサンプリング](http://discoverybiz.net/enu0/faq/faq_YUVSubSampleByBreeze.html)に関する情報
    * 色空間変換時のPSNR比較: [Quality of RGB-YUV-RGB conversion](http://discoverybiz.net/enu0/faq/faq_YUVbyBreeze_test_00.html). 
* __フレームレート理論__:
  * [人間が認識可能なフレームレート](https://www.100fps.com/how_many_frames_can_humans_see.htm), [PDF](//yukisubs.files.wordpress.com/2016/11/how_many_fps_can_the_human_eye_see.pdf).
    * この理論ガイドではぼかしや輝度による主観的な滑らかさにも言及している。
  * [FFmpegのGroup of Picturesオプションを理解する](//esoterictek.blogspot.com/2017/04/understanding-ffmpegs-group-of-pictures.html). 
  * 可変フレームレート: [ファンサブにおけるVFR](//forums.animesuki.com/showthread.php?t=34738), [PDF](//yukisubs.files.wordpress.com/2016/10/vfr_for_fansub_encoders.pdf)
  * AviSynth's [VFRガイド](http://avisynth.nl/index.php/VFR) [VFRaC Workarounds](//mod16.org/hurfdurf/?p=7).
  * FPS理論について実際に動かしながら学習: [frames-per-second.appspot.com](//frames-per-second.appspot.com).
* __インターレース理論__:
  * いくつかの [CRT, NTSC,インターレースの歴史](http://foro.doom9.org/video-basics.htm).
  * すべてを知るためのガイド(非推奨) [interlacing](https://www.100fps.com), [PDF](//yukisubs.files.wordpress.com/2016/11/what_is_deinterlacing_the_best_method_to_deinterlace_movies.pdf).
  * [インターレースTV,フィルムとビデオの変換,その他の事実について](//hometheaterhifi.com/volume_7_4/dvd-benchmark-part-5-progressive-10-2000.html). 
* __コーデックにおけるビット割当理論__:
  * [ビットレート制御を理解する(x264, x265)](http://slhck.info/video/2017/03/01/rate-control.html), [PDF](//yukisubs.files.wordpress.com/2017/04/understanding_rate_control_modes_x264_x265.pdf).
  * [CRF ガイド(レート定数(訳注:品質を指定するための係数) x264 and x265)](http://slhck.info/video/2017/02/24/crf-guide.html), [PDF](//yukisubs.files.wordpress.com/2017/04/crf_guide_constant_rate_factor_in_x264_and_x265.pdf).
  * [x264の設定とビットレートに関するガイド](http://www.lighterra.com/papers/videoencodingh264).
* __解像度理論と基準__:
  * [ネイティブ解像度とスケーリング](//kageru.moe/blog/article/resolutions)と [自動化スクリプト](https://github.com/Infiziert90/getnative).
  * 一般的な解像度に関する怪しい(訳語疑問)リンク:*[random article](https://www.bestusbpoweredmonitor.com/2017/08/16/720p-vs-1080p-vs-1440p-vs-4k-vs-8k/) and [another one](https://www.lifewire.com/720p-vs-1080p-a-comparison-1847332).*
  * [様々な番組のネイティブ解像度](//anibin.blogspot.com/2017/07/blog-post.html).
  * [スケーリング理論とアルゴリズム](//www.cambridgeincolour.com/tutorials/image-interpolation.htm), [Part 2](//www.cambridgeincolour.com/tutorials/image-resize-for-web.htm).
  * 2018年1月における [市販メディアの4kアップスケーリング](https://freetime.mikeconnelly.com/archives/1206).
* __オーディオ理論__:
  * [可聴周波数と聞こえ方:Part1-基礎](https://hometheaterhifi.com/technical/technical-reviews/audio-frequency-loudness-part-introduction-basics/).
  * [実際の音と周波数構成:Part2](https://hometheaterhifi.com/technical/technical-reviews/real-sounds-frequency-composition-part-ii).
* __エンコードとリリース基準__: これらは一般社会におけるデコーディングの互換性を確保するために存在する。アニメコミュニティでは互換性が重視されないことが多い。
  * Apple's [General Authoring Requirements](//developer.apple.com/library/content/documentation/General/Reference/HLSAuthoringSpec/Requirements.html#//apple_ref/doc/uid/TP40016596-CH2-SW1).
  * Youtube's [Recommended upload encoding settings](//support.google.com/youtube/answer/1722171?hl=en).
  * "Scene" [release standards](//scenerules.org) for [Anime](//scenerules.org/n.html?id=2014_X264-ANIME.nfo),  [x264](//scenerules.org/n.html?id=2011_X264.2.nfo), [DVDrips](//scenerules.org/n.html?id=2011_DVDR.nfo), [BDrips](//scenerules.org/n.html?id=2010_BDr.nfo).
  * Microsoft's [Video Media Types](//docs.microsoft.com/en-us/windows/desktop/medfound/video-media-types) and [supported formats](//docs.microsoft.com/en-us/windows/desktop/medfound/supported-media-formats-in-media-foundation).
* __具体的なガイド (雑多)__:
* Koby/Finayraの具体的な [初心者ガイド](//tofincayra.wordpress.com/encoding/beginners-guide), クイックスタートから最新技術まで。このガイドはToDoの翻訳。eXnebducのガイドは16bitフィルタリングまでカバー
* [HuffYUVをWindowsにインストールする方法](http://www.digitalfaq.com/forum/video-conversion/2193-cannot-install-huffyuv.html#post11627).
* [Doom9フォーラム](http://forum.doom9.org/index.php) と [ガイドインデックス](http://foro.doom9.org/guides.htm).
* DVDビデオ(VOB)ファイルの正確なフレームインデックス作成: [DGIndex](http://avisynth.nl/index.php/DGDecode) を [AviSynth](http://avisynth.nl/index.php/Main_Page)で利用。:[関連ガイド](//www.animemusicvideos.org/guides/avtech/videogetb2.html).
* [エンコードに関するヒント](https://sites.google.com/site/taumox/encoding-tips-for-mini-size).
* [雑多な変換に関する目次](http://www.videohelp.com/guides/category/convert-articles-4;43) と Afterdawnの[ガイドインデックス](http://www.afterdawn.com/guides/guides_by_category.cfm).
* [モニターキャリブレーション](//www.cambridgeincolour.com/tutorials/monitor-calibration.htm).
* pixelblendedの[AMV 101](https://pixelblended.com/amv101/en/).
* l33tmeatwadの[ソフトウェアリスト](//www.animemusicvideos.org/forum/viewtopic.php?t=124965)と [AMVtool](https://github.com/l33tmeatwad/AMVtool).
* DarkDream787のエンコードチュートリアル (PDF):
  * [要求ソフトウェア](//yukisubs.files.wordpress.com/2017/06/darkdream787-tutorials-required-software-list.pdf).
  * バックアップ法 [DVDからHDD](//yukisubs.files.wordpress.com/2017/06/how-to-backup-dvds-to-hdd.pdf)と [Blu-RayからHDD](//yukisubs.files.wordpress.com/2017/06/how-to-backup-blu-rays-to-hdd.pdf).
  * SRT,ASSといった字幕を [DVDs](//yukisubs.files.wordpress.com/2017/06/how-to-create-srt-or-ass-subtitles-from-dvd.pdf) や [Blu-Rays](//yukisubs.files.wordpress.com/2017/06/how-to-create-srt-or-ass-subtitles-from-blu-rays.pdf)から取り出す方法
  * [DVDやBDから高品質な音声をエンコードする方法](//yukisubs.files.wordpress.com/2017/06/how-to-encode-high-quality-audio-from-dvds-and-blu-rays.pdf).
  * [AVISynthの使い方](//yukisubs.files.wordpress.com/2017/06/how-to-use-avisynth.pdf).
  * [AVISynthのスクリプトをMeGuiでエンコードする方法](//yukisubs.files.wordpress.com/2017/06/how-to-encode-avisynth-scripts-in-megui.pdf).
  * [ビデオとオーディオのカット、分割、結合](//yukisubs.files.wordpress.com/2017/06/cutting-splitting-merging-video-and-audio.pdf).
  * [動画・音声・字幕ファイルからMKVファイルを作成する方法](//yukisubs.files.wordpress.com/2017/06/how-to-make-an-mkv-file-from-video-audio-and-subtitle-files.pdf).
* 雑多なソフトウェア: [エンコード経験者に聞く](//dustorrent.com/community/show/ask-experienced-encoder-here), [PDF](//yukisubs.files.wordpress.com/2016/10/ask_an_experienced_encoder.pdf).
* 具体的なソフトウェア一覧 (上に近いほど使いやすく、下に近いほど機能が充実)
  * [Handbrake](//handbrake.fr), と[ガイド](//lifehacker.com/5559007/the-hassle-free-guide-to-ripping-your-blu-ray-collection).
  * vEncode [プロジェクトページ](//github.com/gdiaz384/vEncode) and [リリースページ](//github.com/gdiaz384/vEncode/releases). ちなCLI
  * [MeGUI](http://www.videohelp.com/software/MeGUI), [Project Thread](http://forum.doom9.org/showthread.php?t=96032), and [Guide](http://www.sevenforums.com/tutorials/104382-video-encoding-x264-megui.html), [PDF](//yukisubs.files.wordpress.com/2016/10/video_encoding_x264_with_megui.pdf).
  * StaxRip: [VideoHelp page](//www.videohelp.com/software/StaxRip), [GitHub Project Page](//github.com/stax76/staxrip), and [Handbook](//www.gitbook.com/book/stax76/staxrip-handbook/details).
  * [Hybrid](http://www.videohelp.com/software/Hybrid) GUIサポートあり
    * __FFMPEG__: 
      * Getting Started: [FFmpeg: 究極のビデオ・オーディオ操作ツール](//blog.superuser.com/2012/02/24/ffmpeg-the-ultimate-video-and-audio-manipulation-tool/), [PDF](//yukisubs.files.wordpress.com/2017/04/ffmpeg_the_ultimate_video_and_audio_manipulation_tool.pdf).
      * Getting Started 2: [ FFmpegを使ったビデオとオーディオの変換の手引き](http://www.hongkiat.com/blog/ffmpeg-guide).
      * [便利なFFmpegコマンド](http://www.labnol.org/internet/useful-ffmpeg-commands/28490).
      * [FFmpegとH.264のエンコードガイド](//trac.ffmpeg.org/wiki/Encode/H.264).
      * [ビデオに字幕を書き込む方法](//trac.ffmpeg.org/wiki/HowToBurnSubtitlesIntoVideo).
      * 公式[ダウンロード](//ffmpeg.org/download.html), [Windowsへのクロスコンパイル](//trac.ffmpeg.org/wiki/CompilationGuide/CrossCompilingForWindows), [ビルドヘルパースクリプト](//github.com/rdp/ffmpeg-windows-build-helpers), and Todo: nvenc compile guide and [3.2 binaries].
      * [FFmpeg wiki](//trac.ffmpeg.org/wiki), 公式 [難解なDocumentation](//ffmpeg.org/ffmpeg.html), cryptic [Arch Docs](//wiki.archlinux.org/index.php/FFmpeg).
      * 発展的な [複数出力ガイド](//trac.ffmpeg.org/wiki/Creating%20multiple%20outputs) (同時に480p, 720p, and 1080p みたいなエンコード).
  * [x264 Project Page](//www.videolan.org/developers/x264.html), [Documentation](http://www.chaneru.com/Roku/HLS/X264_Settings.htm), and [binaries](//download.videolan.org/x264/binaries).
  * [x265 Information](http://x265.org), [Documentation](//x265.readthedocs.io/en/default/introduction.html) and [binaries](http://msystem.waw.pl/x265).
* __音声エンコーディング__:
  * [FFMPEG 高品質オーディオガイド](//trac.ffmpeg.org/wiki/Encode/HighQualityAudio).
  * [eac3to](http://www.videohelp.com/software/eac3to): コマンドラインインタフェース(CLI)のオーディオエンコーディングツールで、多くのグラフィカルユーザインタフェース(GUI)が利用できます
  * DarkDream787's [DVD/BDから高音質オーディオをエンコードする方法](//yukisubs.files.wordpress.com/2017/06/how-to-encode-high-quality-audio-from-dvds-and-blu-rays.pdf).
  * Opus codec [の比較](//opus-codec.org/comparison)と [FAQ](//wiki.xiph.org/OpusFAQ).
* __再生 (パソコン)__:
  * DVDの再生、映像の分析やストリーミングの保存に使用。通常の視聴にはしようしない: [VLC Media Player](//www.videolan.org/index.html).
  * Windowsなら以下の一つをインストール (MPCとLAVが自動的にインストールされる):
    * [Combined Community Codec Pack (CCCP)](http://www.cccp-project.net). (軽量だが再生専用)
    * [K-Lite Codec Pack](//www.codecguide.com/download_k-lite_codec_pack_mega.htm). (エンコーダ用のVFWコーデックを含むメガパック)
    * [Kawaii Codec Pack (KCP)](http://haruhichan.com/forum/showthread.php?7545-KCP-Kawaii-Codec-Pack).
  * [MediaInfo](//sourceforge.net/projects/mediainfo)はK-Lite CPとともに自動的にインストールされます。それ以外の場合は、必要に応じて手動でインストールすること。
  * [mpv](//mpv.io), [prescalers](//github.com/bjin/mpv-prescalers)は MPlayer のモダンフォーク。 mpv [FAQ](//github.com/mpv-player/mpv/wiki/FAQ), [Wiki](//github.com/mpv-player/mpv/wiki), Moodkillerによる [ガイド](//kametsu.com/topic/63120-mpv-made-easy-moodkiller-edition) and Kokominsによる [ガイド](//kokomins.wordpress.com/2019/10/14/mpv-config-guide/).
    * [MPlayer](//www.mplayerhq.hu)はクロスプラットフォームのメディアプレイヤー。 ArchLinuxの[ドキュメント](//wiki.archlinux.org/index.php/MPlayer)と 公式 [technical documentation](//www.mplayerhq.hu/DOCS/HTML/en/index.html).
    * [SMPlayer](https://www.smplayer.info/) はmpv のラッパーとして設定可能なクロスプラットフォームのメディアプレイヤー。 MPC-HC と似たような UI を持っている。
  * 高度なヒント [LAV splitter stream selection](https://1f0.de/lav-splitter/lav-splitter-stream-selection/).
  * [madVR](http://madvr.com), [FAQ](http://forum.doom9.org/showthread.php?t=146228),(GPUレンダラー)は、デフォルトの設定に比べて、より忠実にビデオを表示することができます。また、シャープネスや色調補正などのリアルタイムフィルターにも対応しています。実装は、MPC-HCやmpvなど様々なプレーヤーのWindowsプラグインとして行われている。K-Lite Codec Packと一緒に自動インストールされるか、手動でインストールされた後、プレーヤー内で使用するために選択する必要があるため、以下のようなガイドがあります。
    * Kametsu guide for [MPC-HC + LAV/madVR/xy-subfilter](//kametsu.com/topic/58428-guide-installing-mpc-hc-with-madvr-lavfilters-xysubfilter-and-icaros).
    * Or for mpv: [Scum's Raws guide](//iamscum.wordpress.com/videoplayback-guide).
    * Some more: [ranpha's PotPlayer guide](//imouto.my/tutorials/configuring-potplayer-for-gpu-accelerated-video-playback-with-dxva-or-cuda-and-also-high-performance-software-decoding/), [BakaBT Wiki](http://wiki.bakabt.me/index.php/Hi10P), [CoalGirls - 2011](//coalgirls.wakku.to/faq/playback/setup-guide-for-mpc-hc-madvr), [another one](//shittastes.wordpress.com/tutorials/properly-installing-and-setting-up-mpc-hc/) and finally [Nand's Guide](http://haruhichan.com/wpblog/205/hi10p-info-guide/), [mirror](http://archive.is/VnjWi), [PDF](//yukisubs.files.wordpress.com/2018/02/hi10pforanimefans_and_playbackguide_bynand_haruhichan.pdf).
    * Advanced: ranpha's very detailed [madVR settings configuration guide](//imouto.my/tutorials/madvr/), [PDF](//yukisubs.files.wordpress.com/2018/02/madvrconfiguration_-by_ranpha.pdf).
* *__Playback (HTPC)__:*
  * *Remote: Use [this](//www.amazon.com/Windows-Control-Infrared-Receiver-Ultimate/dp/B00224ZDFY/ref=sr_1_1?ie=UTF8&qid=1334779407&sr=8-1), or*
  * *A [wireless keyboard](//www.amazon.com/s/ref=nb_sb_noss?url=search-alias%3Delectronics&field-keywords=logitech+wireless+keyboard+with+touchpad), [mini version](//www.ebay.com/sch/i.html?_from=R40&_trksid=p2380057.m570.l1313.TR12.TRC2.A0.H0.Xmini+wireless+keyboard.TRS0&_nkw=mini+wireless+keyboard&_sacat=0).*
  * *For a dedicated HTPC box: [Kodi](//kodi.tv) (formally XBMC).*
    * *Note: Natively, the Raspberry Pi 3 B cannot properly decode 10-bit content.*
    * *Notable Variants: [LibreElec](//libreelec.tv), [OpenElec](http://openelec.tv/), [Plex](//www.plex.tv).*
  * *For a Client-Server model (recommended): either [Plex](//www.plex.tv) (closed source) or [Emby](//emby.media), formally Media Browser, (open source).*
    * *Plex/Emby realtime transcoding (free) means all client devices will always be able to decode streams properly (universal compatibility, including HTML5 web browsers).*
    * *Notable Variants: [RasPlex](http://www.rasplex.com), [Kodi's Plex Add-on](//kodi.tv/plex-add-on-for-kodi), and the Plex Client for Xbox 360.*
    * *Plex's [Full Client List](//forums.plex.tv/discussion/190573/list-of-current-client-product-and-client-platform).*
    * *Emby's [Kodi addon](//emby.media/emby-for-kodi.html), [repository](//github.com/MediaBrowser/plugin.video.emby/wiki/Emby-Repository) (to install the dependencies), and [Full Client List](http://emby.media/download.html).*
    * *Random: Check out [Rasplex](http://www.rasplex.com/), [Kodi via OpenElec](//openelec.tv/), [Raspian](//www.raspbian.org), and [RetroPi](//retropie.org.uk).*
  * *Or just use an [High-Definition Multimedia Interface](http://www.hdmi.org/consumer/hdmi_advantage.aspx) (HDMI) cable (audio + video) to connect a laptop to a TV temporarily. [HDMI FAQ](http://www.hdmi.org/learningcenter/faq.aspx).*
* __QC__ (?): [Bitrate Viewer](http://www.winhoros.de/docs/bitrate-viewer) Able to estimate the quality of MPEG1 and MPEG2 streams.どこがどう便利なのかわかりませんが、Etzimalが追加しろと言っていました。

#### __多重化と分割__

* __理論__: 多重化(Muxing)は複数の個別ファイル(ビデオ、オーディオ、字幕、フォント)を再生用の1つのファイルに統合すること。 分割(Demuxing)は、複数のストリームを含む1つのファイルを取り出し、そのうちの少なくとも1つを抽出すること。
* 多重化は一般的に、同期のためにストリームを短くしたり、長くしたり、遅らせたりすることがある。短縮や遅延は、ストリームのコピー技術と互換性があるが、カット編集などを行うと通常、ストリーム全体をトランスコードする必要があるので、2つの作業(エンコードと多重化)は多少重なる。
* 分割は通常、作業用のソースを得るために必要であり、キャッピングの一部と考えることができる。
* 一般的に使用されるコンテナは、ソフトサブ(訳注:動画に直接埋め込まれていない字幕),フォント,場合によっては複数のオーディオストリームを備えたMatroska().mkv),またはハードサブと単一のオーディオストリームを備えた標準的なMPEG-4(.mp4)コンテナです。
* __多重化ツール__:
* FFMPEG:
  * スイッチ: `-ss -t -to` を参照せよ。詳細は[ffmpeg documentation](//ffmpeg.org/ffmpeg.html#Main-options) と [ガイド](//trac.ffmpeg.org/wiki/Seeking).
  * マルチストリームファイルで最初ではないファイルを抽出するには `-map` スイッチを用いる。. [FFMPEG documentation](//ffmpeg.org/ffmpeg.html#Advanced-options) と [関連するガイド](//trac.ffmpeg.org/wiki/Map).
* [MKVToolNix](//mkvtoolnix.download/index.html):
  * [VideoHelp 概要](//www.videohelp.com/software/MKVtoolnix).
  * Download: [Windows/OS-X](//www.fosshub.com/MKVToolNix.html), [Linux](//mkvtoolnix.download/downloads.html).
  * Required Add-on: gMKVExtractGUI. [Project Page](http://forum.doom9.org/showthread.php?t=170249) and [DL Link](//sourceforge.net/projects/gmkvextractgui/files/latest/download).
  * MKVMerge's [CLI Documentation](//mkvtoolnix.download/doc/mkvmerge.html).
  * 発展: [Creating Multi-Part Files](http://forum.videohelp.com/threads/359121-How-to-extract-cut-parts-from-a-mkv-including-all-audio-and-subtitle-tracks), [Concatening Multi-Part Files](//forums.plex.tv/discussion/178888/howto-joining-multi-part-movies-files-with-mkvtoolnix-gui).
  * 発展: [Ordered Chapters](https://forums.animesuki.com/showthread.php?t=66444) (OC) summary. Ordered Chaptersは使用しないこと。
    * *[Implementation Details](//mod16.org/hurfdurf/?p=8), [Part 2](//mod16.org/hurfdurf/?p=14).*
    * *To attempt to fix OCs: [UnlinkMKV](//github.com/gnoling/UnlinkMKV).*
  * VFRを扱うなら [外部のタイムスタンプファイル](https://mkvtoolnix.download/doc/mkvmerge.html#mkvmerge.external_timestamp_files)を使用すること。
* DVDs: 
  * [DVD-Decrypter](http://www.videohelp.com/software/DVD-Decrypter), [Mega Download](//mega.nz/#F!wUYwDSgA!8tx_37HUBcs9KqPhkk5FmQ), + [ストリームガイド](http://www.doom9.org/index.html?/dvddec.htm). 依存関係: DVD-Decryptor は [Virtual CloneDrive](//www.elby.ch/en/products/vcd.html)か物理DVDドライブのような光学デバイスが必要です。Video_TSフォルダが利用できる場合(DVDリッピング)ならCDBurnerXPのようなISOファイルを作成できるソフトウェアを使用。
  * DGIndex, [DGDecode](http://avisynth.nl/index.php/DGDecode)の一部。 [dgmpgdec158.zip](//mega.nz/#F!wUYwDSgA!8tx_37HUBcs9KqPhkk5FmQ).
* BDs:
  * After the contents have been dumped, most bdmvs do not require special demuxing tools to handle. ffmpeg and mkvtoolsnix are usually sufficient but muxing tools can be used to speed up processing.
  * [tsMuxer](http://www.videohelp.com/software/tsMuxeR), [Mega](//mega.nz/#F!wUYwDSgA!8tx_37HUBcs9KqPhkk5FmQ). トランスポートストリーム (.ts または .m2ts) をミックスアウトする FFMPEG の代替品。Blu-ray インデックス (mpls) の解析をサポート。
  * [HD-DVD/Blu-Ray Stream Extractor](http://www.videohelp.com/software/HD-DVD-Blu-Ray-Stream-Extractor), [Mega](//mega.nz/#F!wUYwDSgA!8tx_37HUBcs9KqPhkk5FmQ).tsMuxer の代替。これと tsMuxer の両方を使用することを推奨。
  * 注:両方とも [eac3to](http://www.videohelp.com/software/eac3to)が必要。
* [MKV-Cutter](https://www.videohelp.com/software/MKV-Cutter) (untested).
* __Guides__: 
  * OblivionShadowとkantai.subs.moeのガイド: [Advanced SubStation Alpha Merging and Muxing Guide Guide - PDF](//kantai.subs.moe/wp-content/uploads/2016/08/Aegisub-Merging-and-Muxing-Guide.pdf), [PDF](//yukisubs.files.wordpress.com/2018/02/aegisub_merging_and_muxing_guide_by_oblivionshadow.pdf).
  * Baal's [How To: Synchronize Two Audio Tracks For Muxing With Audacity](//kametsu.com/topic/45949-how-to-synchronize-two-audio-tracks-for-muxing-with-audacity).
  * Catar's [Standards of Muxed Releases](//kametsu.com/topic/62012-the-ctr-muxing-standards-guide). 注:メディアサーバーと互換性のあるデュアルオーディオのリリースに重点を置いている。

#### __フィルター__

* __始める前に__:何度もトランスコードしたり、ロスレスにエンコードされた映像を転送したりするのを避けるためには、フィルタリングとエンコードを同じ人が行うのが理想的。
* __理論__: [IVTC](http://foro.doom9.org/ivtc-tut.htm) (逆テレシネ)を超えるフィルタリングタスクは、エンコーダのオプションのサブタスクと考えることができます。一般的なフィルタリング作業には、長さのトリム、広告のカット、スタジオの様々なミスの修正、主観的な視覚品質の改善などがあります。
* 互換性を気にするエンコーダーは、OP/EDやスクリプト全体をディストロの前にビデオストリームにハードサブする必要があるかもしれません。これは、フィルタリングとエンコードのどちらの段階でも行うことができます
* 基本的な作業を超えると、フィルタリングはあまり効果がありません。習得にも実装にも非常に時間がかかります。
* 追加情報: 
* RX Masteringの [ビデオ哲学](https://rxmastering.wordpress.com/video).
* [DVDにおけるデジタルノイズリダクション:背景と実例](http://www.cinedrome.ch/hometheater/dvd/dnr).
* 理論と実例のミックス [Digital ICE](//www.youtube.com/watch?v=E0LVjGp1Wtc) (YouTube).
* __実例__:
  * ビデオ修復: [Avisynthの威力 Part III](https://vimeo.com/11133342)とデジタル化 [8mm film](https://vimeo.com/49963017) (vimeo).
  * [精霊の守り人](http://compare.bakashots.me/compare.php?setId=2089), [Kiss×sis OVA](http://compare.bakashots.me/compare.php?setId=1973&comparisonId=12625), [超次元ゲイム ネプテューヌ](http://compare.bakashots.me/compare.php?setId=2028&comparisonId=13099) (all overfiltered but w/e).
  * Moozzi2'の「落第騎士の英雄譚」 [Before](//yukisubs.files.wordpress.com/2016/10/moozzi2_rakudai_1_before.png) [After](//yukisubs.files.wordpress.com/2016/10/moozzi2_rakudai_1_after.png).
  * 微妙のフィルター: [Case Study: Turn-A Gundam](//rxmastering.wordpress.com/2014/12/03/case-study-turn-a-gundam/).
  * [NeatVideo](//www.neatvideo.com/examples) - similar to [TemporalDegrain()](http://avisynth.nl/index.php/Temporal_Degrain) for AviSynth.
  * [Improving Visual Quality with AviSynth Filters](https://www.animemusicvideos.org/guides/avtech31/post-qual.html), [PDF](//yukisubs.files.wordpress.com/2016/10/amv_post_production_-_visual_quality.pdf).
  * [Using Filters and Functions](http://www.l33tmeatwad.com/vapoursynth101/using-filters-functions) (Vapoursynth).
* __Understanding and Identifying Artifacts__:
  * [Understanding Video Compression Artifacts](http://blog.biamp.com/understanding-video-compression-artifacts/).
  * [Macroblocking vs Mosquito noise](https://hometheaterhifi.com/volume_12_1/algolith-mosquito-video-noise-reducer-3-2005.html).
  * [Depth of Field](//www.cambridgeincolour.com/tutorials/depth-of-field.htm) and [Hyperfocal Distance](//www.cambridgeincolour.com/tutorials/hyperfocal-distance.htm) theory.
  * [Understanding Camera Lenses](//www.cambridgeincolour.com/tutorials/camera-lenses.htm).
    * Using the wrong color matrix while filtering can result in either "Loss of Contrast" or "Vignetting."
    * Upscaling creates "Blurring."
    * warp sharpening and stabilization create "Distortion."
    * Improper capture settings or equipment, especially for analog video, can create "chromatic aberrations" or "rainbowing".
  * [Digital Camera Image Noise - Part 1](//www.cambridgeincolour.com/tutorials/image-noise.htm), and [Part 2](//www.cambridgeincolour.com/tutorials/image-noise-2.htm).
  * [Guide to Image Sharpening](//www.cambridgeincolour.com/tutorials/image-sharpening.htm).
  * TODO: Dot crawl, banding
* __Frameworks__:
  * [__AviSynth__](http://avisynth.nl/index.php/Main_Page):
    * [AviSynth+](http://avs-plus.net/) (64-bit) and Github [releases page](//github.com/pinterf/AviSynthPlus/releases).
    * l33tmeatwad's [AviSynth 101](http://www.l33tmeatwad.com/avisynth101).
    * [Scintilla's Guide to AviSynth Postprocessing Filters](http://www.aquilinestudios.org/avsfilters/index.html), [PDF](//yukisubs.files.wordpress.com/2016/10/scintilla_guide_to_avisynth_postprocessing_filters.pdf).
    * [Filtering the PPP way](https://www.otakubell.com/?page_id=291) by erik.
    * Syntax: 
      * [My First AviSynth Script](http://avisynth.nl/index.php/First_script), and [FAQ](http://avisynth.nl/index.php/AviSynth_FAQ).
      * [Script Examples](http://avisynth.nl/index.php/Script_examples), and another [random example](http://pastebin.com/jDuP5STF) (was overfiltered but w/e).
      * AviSynth [CopyFromMe Template](//gist.github.com/YukinoAi/36a9f4c0deb193b1113c8fd10d5d8fc7).
      * An advanced [16-bit filtering template](//tofincayra.wordpress.com/encoding/basic-avisynth-script).
    * Filter lists: 
      * [Internal Filters](http://avisynth.nl/index.php/Internal_filters).
      * [External Filters](http://avisynth.nl/index.php/External_filters).
      * [MSU Public Filters](http://www.compression.ru/video/public_filters.htm).
      * real.finder's [Index](//forum.doom9.org/showthread.php?t=174121).
      * josemaria.alkala's [random x86 filters](//bitbucket.org/josemaria.alkala/avisynth_filters/src).
      * StainlessS's [repository](//www.mediafire.com/folder/hb26mthbjz7z6/StainlessS).
    * Misc:
      * [nnedi3](http://avisynth.nl/index.php/Nnedi3), [binaries](https://github.com/jpsdr/NNEDI3/releases/), and [nnedi3_resize16](https://www.nmm-hd.org/newbbs/viewtopic.php?f=7&t=1117). "[...] NNEDI3, which was originally designed as an intrafield deinterlacer[, ...] is also useful for enlarging images by powers of two. Compared to earlier NNEDI versions, v3 has an improved predictor neural network architecture and local neighborhood pre-processing. NNEDI3’s neural network consists of 16 to 256 neurons. 32 neurons generally has the best quality for performance." -[src](https://freetime.mikeconnelly.com/archives/1206)
      * [Hysteria](//www.animemusicvideos.org/forum/viewtopic.php?t=101471). Line darkner.
      * ["Tweak" guide](http://avisynth.nl/index.php/Tweak) for fine adjustment of colors. Hint: Use maxsat=15-35.            
      * [Histogram](http://avisynth.nl/index.php/Histogram), [alternative](http://avisynth.nl/index.php/Histograms_in_RGB_%26_CMY). Useful for analyzing colors shifts in color families without separate luma.
      * [Smooth Video Project (SVP)](https://www.svp-team.com/wiki/Download), [Manual](//www.svp-team.com/wiki/Manual:SVPflow), for frame interpolation.  Works with VapourSynth as well.
      * [SmoothAdjust](//forum.doom9.org/showthread.php?t=154971). Makes YUV color adjustments. Also see: [Autolevels](http://www.thebattles.net/video/autolevels_comparison.html) and [GamMac](//forum.doom9.org/showthread.php?t=173695), [2](http://www.filmshooting.com/scripts/forum/viewtopic.php?t=27143).
      * [WhiteBalance](http://avisynth.nl/index.php/WhiteBalance).
      * [AviSynth Shader](//github.com/mysteryx93/AviSynthShader). Used to run HLSL pixel shaders that have not been natively ported.
      * [TemporalDegrain2](//forum.doom9.org/showthread.php?s=4c6011fbc9f07c5bdbced4d27dce5cdd&t=175798).
  * [__VapourSynth__](http://www.vapoursynth.com/about/): alternative to AviSynth with many cross-compatible filters. Requires [Python 3.8](//www.python.org/downloads/release/python-385/).
    * l33tmeatwad's [VapourSynth 101](http://www.l33tmeatwad.com/vapoursynth101) and [Using Filters and Functions](http://www.l33tmeatwad.com/vapoursynth101/using-filters-functions).
    * Official doc's [installation](http://www.vapoursynth.com/doc/installation.html), and [Getting Started](http://www.vapoursynth.com/doc/gettingstarted.html). l33tmeatwad's [VapourSynth Install Guide](//www.animemusicvideos.org/forum/viewtopic.php?t=125039).
    * eXmendiC's [Filtering With VapourSynth](//iamscum.wordpress.com/encoding-stuff/filtering-with-vapoursynth), [PDF](//yukisubs.files.wordpress.com/2017/09/filtering_with_vapoursynth_by_exmendic.pdf).
    * Ausna/Yuuki's [Vapoursynth + x265](https://blog.mxpkx.com/index.php/archives/144/), [PDF - Eng](https://yukisubs.files.wordpress.com/2020/04/vapoursynth_x265_by_yuuki.pdf), setup guide.
    * Encoding from .vpy files is done using [vspipe.exe](http://www.vapoursynth.com/doc/vspipe.html). Options:
      1. See [this guide](//iamscum.wordpress.com/encoding-stuff/x264-encoding-with-vapoursynth).
      2. Use an ffmpeg/x264/x265 frontend like [vEncode](//github.com/gdiaz384/vEncode) that incorporates vspipe.exe. See the "Encoding: Specific Software" section for alternatives.
      3. Interlace the .vpy in a .avs file and encode as a normal .avs file. See [VapourSource](http://avisynth.nl/index.php/VapourSource).
    * Filter lists:
      * [Official Plugins List](http://www.vapoursynth.com/doc/pluginlist.html) (includes [BM3D](//github.com/HomeOfVapourSynthEvolution/VapourSynth-BM3D) and [waifu2x-caffe](//github.com/HomeOfVapourSynthEvolution/VapourSynth-Waifu2x-caffe)).
      * VapourSynth Evolution's [Filter Index](//github.com/HomeOfVapourSynthEvolution).
      * HolyWu's [HAvsFunc ported function list](//forum.doom9.org/showthread.php?t=166582).
      * Irrational-Encoding-Wizardry's [Github Homepage](//github.com/Irrational-Encoding-Wizardry). Motto: "A bunch of autists making encodes better for muggles."
      * vfrmaniac's ["works" index](https://vfrmaniac.fushizen.eu/works/) (includes FFT3DFilter binary).
      * [InsaneAA](//github.com/Beatrice-Raws/VapourSynth-insaneAA).
    * Vapoursynth [CopyFromMe Template](//gist.github.com/YukinoAi/fa90db376296d5673fd2a2f0e4442ee3).
    * BeatriceRaw's [encode-scripts](//github.com/Beatrice-Raws/encode-scripts), related Sword Art Online II [example scripts](//github.com/Jensenbeatrice/Sword-Art-Online-II-scripts).
  * [__VirtualDub__](http://virtualdub.org/index.html), [v2](//www.videohelp.com/software/VirtualDub2):
    * [Interesting History](http://www.virtualdub.org/virtualdub_history.html).
    * For stabalization: [Deshaker](http://www.guthspot.se/video/deshaker.htm), [PDF](//yukisubs.files.wordpress.com/2018/02/deshaker-video-stabilizer.pdf).
      * [Random youtube video](//www.youtube.com/watch?v=nIo_AuYRVj0) on Deshaker
      * Todo: some sane example settings go here.
        * Color correction: [ColorMill](http://fdump.narod.ru/rgb.htm) and [guide](http://www.infognition.com/tutorials/color_correction/).
* Additional programs used:
  * [AvsPmod](//avspmod.github.io), Integrated Development Enviornment (IDE) for AviSynth and VapourSynth. todo: put additional DDL link here.
  * VapourSynth Editor (vsedit), Alternative IDE for VapourSynth. [Thread](//forum.doom9.org/showthread.php?t=170965) and [Project Page](//bitbucket.org/mystery_keeper/vapoursynth-editor).
  * [Yunno](//yuuno.encode.moe) = [Jupyter](//jupyter.org) + VapourSynth. Alternative IDE to vsedit. Additional dependencies: [Jupyter](//jupyter.org/install.html) and [iPython](//ipython.readthedocs.io/en/stable/install/index.html).
  * Note: [MPC-x86-Portable](//mpc-hc.org/downloads), or the 64-bit version if using AviSynth+, can load .avs files directly.
  * Waifu2x for upscaling and/or denoising.  
    * See [combined example results](http://diff.pics/nmS9GmlpSUV7/5) and [upscaling component only example](//diff.pics/vJ5W2v4l0q9y/1).
    * Note: Some caffe versions of waifu2x can use nvidia's CUDA Deep Neural Network (CUDNN) library instead of OpenCL/AVX. These versions are faster but require 64-bit Windows, a [CUDNN capable GPU](//developer.nvidia.com/cuda-gpus), i.e. compute capability 3.0+, and [nvidia_CUDNN.dll.7z](//mega.nz/#F!wUYwDSgA!8tx_37HUBcs9KqPhkk5FmQ). Most versions also have a "CPU only" mode.
    * [waifu2x-caffe-VapourSynth](//github.com/HomeOfVapourSynthEvolution/VapourSynth-Waifu2x-caffe) variant for VapourSynth that supports CUDA/CUDNN.
    * [waifu2x-caffe-VapourSynth-w2xc](//github.com/HomeOfVapourSynthEvolution/VapourSynth-Waifu2x-w2xc) variant for VapourSynth that supports OpenCL 1.2.
      * [waifu2x-caffe](//github.com/lltcggie/waifu2x-caffe) standalone variant that supports CUDNN that can work with video as an image sequence. Important: This version also contains the /models folder required by the VapourSynth variants above.
      * [waifu2x-converter-cpp](//github.com/tanakamura/waifu2x-converter-cpp) and [DeadSix27's Fork](//github.com/DeadSix27/waifu2x-converter-cpp) is an older CLI standalone (no framework) CUDA/OpenCL/AVX implementation. [koroshell GUI](http://inatsuka.com/extra/koroshell/).
      * [AutoWaifu](//autowaifu.azurewebsites.net).
* Further reading:
  * [kageru.moe/blog/encode](//kageru.moe/blog/encode/).
  * Abstract: [Javascript Video Filtering](//tp7.github.io/articles/javascript-video-filtering).
* __Scene Filtering__: This is an optional subcomponent of filtering which is an optional sub-component of encoding, which is an optional sub-component of capturing. In other words, stay away.
  * Basic: frameTools's sceneFilter(). See the [documentation](//github.com/gdiaz384/frameTools) and [releases page](//github.com/gdiaz384/frameTools/releases).
  * More efficient and recommended: tp7's [Efficient scenefiltering with AviSynth](//tp7.github.io/articles/scenefiltering), [PDF](//yukisubs.files.wordpress.com/2017/09/efficient-scenefiltering_with_avisynth_by_tp7.pdf).
    * [RemapFrames](http://avisynth.nl/index.php?title=RemapFrames), [PDF guide](//yukisubs.files.wordpress.com/2018/02/remapframes_041.pdf), Groucho's [AviSynth binary](https://forum.doom9.org/showthread.php?t=173259) and Frechdachs's [VapourSynth script](//gist.github.com/Frechdachs/353f6917d78bb99d93bfcea0f29062ed#file-fvsfunc-py-L822).
* __Working with Groups of Pictures (GOPs)__: Scene filtering can also be done in [Photoshop](//www.photoshop.com/products/photoshopelements) or [Gimp](//www.gimp.org) one frame at a time. Manually editing each frame could be described as an optional component of scene-filtering.
* Mandatory reading: [Understanding FFMPEG's Group of Pictures (GOP) Options](//esoterictek.blogspot.com/2017/04/understanding-ffmpegs-group-of-pictures.html).
* Cambridge colour's [Photo Editing Tutorials](//www.cambridgeincolour.com/photo-editing-tutorials.htm) and [Digital Photo Restoration](//www.cambridgeincolour.com/tutorials/digital-photo-restoration.htm).
* Adobe's Photoshop [Retouch and repair photos](//helpx.adobe.com/photoshop/using/retouching-repairing-images.html) user guide.
* Reanimating panning scenes:
  * This can be done to fix stuttering and flickering.
  * [Panorama basics](//www.cambridgeincolour.com/tutorials/digital-panoramas.htm)
  * [How to Auto-Align Layers](https://www.dummies.com/software/adobe/photoshop/how-to-auto-align-layers-in-photoshop-cs6/) 
  * [Use Content-Aware Fill](//www.youtube.com/watch?v=nXVY92gazvE), YT video. At this stage, it is possible to switch to Premiere/Blender.
  * [How to Pan And Zoom in Photoshop CS6](https://www.youtube.com/watch?v=kM5pIHS5j74), YT video. 
* Example: Maybe-not-so-sane [workflow diagram](//i.imgur.com/RGoR1mV.png). Think of this as an example what not to do.
* Special Note: When converting between YUV and RGB, double-check for color distortions manually through every step in the workflow where colorspace conversions between color families occur. This especially applies to denoising algorithims like waifu2x and BM3D (including when using it inside of mvsfunc's wrapper).
* Exporting/Importing Images:
  * FFMPEG image sequence [guide 1](//en.wikibooks.org/wiki/FFMPEG_An_Intermediate_Guide/image_sequence), [guide 2](http://hamelot.io/visualization/using-ffmpeg-to-convert-a-set-of-images-into-a-video/), [guide 3](//trac.ffmpeg.org/wiki/Create%20a%20video%20slideshow%20from%20images).
  * [VirtualDub](http://www.virtualdub.org/blog/pivot/entry.php?id=34) "File-Open video file...," or "File-Export-Image sequence..." (not recommended).
  * [mplayer example](https://superuser.com/questions/135117/how-to-convert-video-to-images) and see the -vo "jpeg" or "png" section of MPlayer's [Video Output Drivers (MPlayer Only) documentation](//www.mplayerhq.hu/DOCS/man/en/mplayer.1.html#VIDEO%20OUTPUT%20DRIVERS%20%28MPLAYER%20ONLY%29) (not recommended).
  * AviSynth:
    * [Image Writer](http://avisynth.nl/index.php/ImageWriter).
    * [ImageReader](http://avisynth.nl/index.php/ImageReader). (terrible)
    * [CoronaReader](http://avisynth.nl/index.php/ImageSequence). (also terrible)
    * [syntax example](//gist.github.com/YukinoAi/bb053f9e4d65155d3123ead9fa03a18e).
* Image Viewers: [InfranView](//www.irfanview.com) or your favorite graphical HTTP client.
* For batch image procesing: [Photoshop Macros](//helpx.adobe.com/photoshop/using/creating-actions.html), [ImageMagick](//www.imagemagick.org/script/command-line-processing.php) (very advanced) and [waifu2x-caffe](//github.com/lltcggie/waifu2x-caffe).
* __Masktools__:
  * [Masktools](http://avisynth.nl/index.php/MaskTools2), [PDF](//yukisubs.files.wordpress.com/2018/02/masktools2_-_avisynth_wiki.pdf), provides an efficent way to select parts of a video frame but not others. If combined with other concepts, like motion compensation and edge detection, masktools allows filters to selectively target aspects within a frame for many consecutive frames. Neither scene filtering techniques, which are clip-based, nor image editing techniques allow for the flexibility and efficency that Masktools can provide.
  * tp7's [MaskTools 2 theory](//tp7.github.io/articles/masktools), [PDF](//yukisubs.files.wordpress.com/2018/02/masktools_2_by_tp7.pdf).
  * tp7's MaskTools for beginners and generally: Translation from Russian: [PDF](//yukisubs.files.wordpress.com/2018/02/masktools_for_beginners_and_generally-tp7.pdf). Link:
    * `http://web.archive.org/web/20160312025423/http://tp7.ruanime.org/masktools/index.html`
  * 06_taro's [MaskTools guide](https://www.nmm-hd.org/newbbs/viewtopic.php?f=7&t=770). Translation from Chinese [PDF - Page 1](//yukisubs.files.wordpress.com/2018/02/tutorial_masktools_getting_started_tutorial_-nmm-hd_1.pdf) and [PDF - Part 2](//yukisubs.files.wordpress.com/2018/02/tutorial_tutorial_for_masktools_-_page_2_-_nmm-hd.pdf).
  * Further reading: [Edge Masks](https://kageru.moe/blog/article/edgemasks/) in Vapoursynth by [Kageru](//github.com/kageru).
* __Real-time filtering__: The idea is to get playback without having to transcode the video.
  * [SmoothVideo Project (SVP)](//www.svp-team.com/wiki/Main_Page), [example](//www.youtube.com/watch?v=4J1PYWCJ6tE), for frame interpolation to 60fps. Note: Avisynth/Vapoursynth plugins also available.
  * Media player GPU accelerated "shaders": [MPC-HC](https://forum.videohelp.com/threads/372235-Is-there-a-way-to-Paste-MPC-HC-shader-effect-to-a-video), [mpv]. Includes sharpening and scaling filters.
  * MadVR has quite a few.
  * With a powerful enough computer and a computationally light enough filter chain, .avs files (AviSynth) can be played directly.

#### __翻訳と検証__

* __Transliterating__: Change the words (and maybe grammar) to a new language.
  __vs__
* __Translating__: Change what was said, including metaphors, to convey the same meaning.

#### __編集とチェック__

* __Editing__: Editors make sure the translation can be easily understood, sounds natural, is consistent and either localized or unlocalized (depending on preference).
* The only requirement for editing is the one must speak the target language fluently, which can be a high bar.
* Personally, I also listen to the foreign audio to make sure the post-edited dialogue stays as literal as possible and make sure the dialogue word choice and typesetting are compatible with [speed reading](//en.wikipedia.org/wiki/Speed_reading) techniques.
* Random: For comprehension, it deosn’t enve mttaer in waht oredr the ltteers in a wrod are bscsaue the hamun brian is well adeptad to roecginze pettarns. Speed reading is the same concept, but applied to sentences instead of individual words. With "[visual reading](http://slowanime.com/is-kanji-still-needed-in-modern-japan)" in English, shorter words (to, a, be, are, by) are grammar that can be skipped by parsing only the longer words. Any "missing" meaning is derived from context. Try reading by skipping all the smaller words. If the sentence does not make sense, change the order and words used so it does make sense. Within this context, contractions are evil.
* tun's [Fansub Editing Guide](http://m33w-fansubs.com/editing-guide), [PDF](//yukisubs.files.wordpress.com/2018/02/fansub_editing_guide_by_tun.pdf).
* [Collectr](//collectr.blogspot.com)'s editing tips:
  * [Curmudgeonly Guide to Editing](//collectr.blogspot.com/2011/01/collectrs-curmudgeonly-guide-to-editing.html), [PDF](//yukisubs.files.wordpress.com/2017/09/collectr_blogs_curmudgeonly_guide_to_editing.pdf).
  * [Editorial Minimalism](//collectr.blogspot.com/2013/10/editorial-minimalism.html), [PDF](//yukisubs.files.wordpress.com/2017/09/collectrs_blog_-editorial_minimalism.pdf).
  * [The Dangers Of Second Hand Translations](//collectr.blogspot.com/2012/12/the-dangers-of-second-hand-translations.html), [PDF](//yukisubs.files.wordpress.com/2017/09/collectrs_blog_the_dangers_of_second-hand_translations.pdf).
* __Important__: Figure out what type of editing you like. 1) Standard-Informal English, 2) Unlocalized literal, or 3) Localized memesubs. [PNG GUIDE](//yukisubs.files.wordpress.com/2017/09/editing_style_comparison-mod.png). Summary:
  1. Unlocalized-Literal: Doki/Eclipse.
  2. Official Standard or Informal English: Crunchyroll, Funimation, official DVD-BD are a close second.
  3. Localized: Commie/DesuYo/FFF are heavily localized memsubs. Avoid unless you knowingly like localization. They are good sources for sign typesetting when combined with dialogue from 1-2 above.
  4. Hadena subs are so not even funny to the point where it is not even not funny anymore and becomes funny again. 
     * Note: The point here is not to comment on Hadena, but rather as to counter editorial minimalism. If the subs are good, leave them alone, but if they are really bad, then change everything.
  5. A lot of remuxers combine existing subs with better/worse Audio and Video (A/V). The subs quality is usually the same as whoever they ripped them from.
  6. Censoring exists (sex-gore), in both dialogue and in A/V. Be wary of this from broadcast streams, especially non-Japanese ones, including older DVDs.
* Use Crymore's [Translation Parties](http://www.crymore.net/category/translation-party/) to figure out what type of editing you like, start with [this one](http://www.crymore.net/2016/01/18/translation-party-commie-vs-doki-chihiro-vs-funimation-vs-mori-dagashi-kashi-episode-01). They take a while but will save time later on by being able to start from "better" subs and having to edit them less overall.
* Blog about fansub drama and editing: [crymore.net](//www.crymore.net).
* __QC__: [Collectr's Curmudgeonly Guide to QC](https://collectr.blogspot.com/search/label/QC).

#### __字幕タイミング__

* Alternative names/sub-categories: Raw Timing, Fine Timing, Scene Timing, Key Frame Timing (KFT), Karaoke Timing (K-Timing).
* [Timing theory](//collectr.blogspot.com/2012/05/its-all-in-timing.html), [PDF](//yukisubs.files.wordpress.com/2017/09/collectrs_blog_its_all_in_the-timing.pdf) by Collectr.
* unanimated's [Timing Basics](//unanimated.github.io/timing-basics.htm), [Timing Without TPP](//unanimated.github.io/timing-without-tpp.htm) and [additional notes](//unanimated.github.io/timing-notes.htm). unanimated's [Fansub Guides](//unanimated.github.io/guides.htm).
* Doki's [Timing Guide](//doki.co/support/doki-timing-guide), [PDF](//yukisubs.files.wordpress.com/2016/10/doki_timing_guide.pdf).
* Sally's [Sally's Guide To Timing Anime](//drive.google.com/open?id=0B0O0wI7T8vtSSldlZHJnUVJaTTA), [PDF](//yukisubs.files.wordpress.com/2017/09/sallys_guide_to_timing_anime.pdf), [GDrive - PDF](//drive.google.com/open?id=0B0O0wI7T8vtSMTBtRDlFNkxIdEE).
  * Resources: [GoogleDrive](//drive.google.com/open?id=0B0O0wI7T8vtSY2hhWmc4RFF3UVE): [Sally's Timing Video](//drive.google.com/open?id=0B0O0wI7T8vtSSm9oaEc0b19YdmM), [Sallys Timing Example](//drive.google.com/open?id=0B0O0wI7T8vtSTU02S0lKRlo2UUk), [picture 1](//drive.google.com/open?id=0B0O0wI7T8vtSMnlrbTlFZjhtOGs) and [picture 2](//drive.google.com/open?id=0B0O0wI7T8vtSRkVJUjFMUUtoUlk).
* WhyNot's [A Guide to Timing in Aegisub](http://whynotsubs.com/A-guide-to-timing-in-Aegisubv2.pdf), [PDF](//yukisubs.files.wordpress.com/2016/10/a-guide-to-timing-in-aegisubv2.pdf).
* m33w-fansubs's [Timing & Styling Guide](http://m33w-fansubs.com/timing_guide.php).
* [skiddiks's](https://yukisubs.files.wordpress.com/2020/09/timing_with_skiddiks_scribbles-1.pdf).
* unanimated's [How to make xvid keyframes](//unanimated.github.io/scxvid.htm).
* For K-timing, the idea is to time the pronouciation of each syllable. If you do not have the [romanticized Japanese syllables](//wiki.anidb.net/w/AniDB_Definition:Romanisation) memorized already, save these Hiragana character maps: [1](//yukisubs.files.wordpress.com/2017/05/hiragana.png) and [2](//yukisubs.files.wordpress.com/2017/05/hiragana3.png).
* Random YouTube videos:
  * [Jude Ibe](//www.youtube.com/watch?v=w6zXR6Bg7fU), [Dozo Douzo](//www.youtube.com/watch?v=nkTbrCYmKPk), and [Govna](//www.youtube.com/watch?v=In7nbmsqHWI&list=PLtwIkfU56fRSZgaPHFt79ei1_Kf4cDaFY&index=11).

#### __字幕組版__

* __Theory__: Typesetting is mostly making sure the subtitle dialogue is visually legible and signs look like they are natively part of the video. Typesetting can also extend to styling the opening, ending and insert songs, including fancy karaoke. [More theory](//collectr.blogspot.com/search/label/typesetting).
* The most important part of typesetting is also the simplest: make sure the dialogue is readable. Check out [Underwater's Styling Guide - PDF](//yukisubs.files.wordpress.com/2018/02/subtitlestyling_byunderwater.pdf). In summary:
  1. Use a very light color as the primary color (white).
  2. Have a very dark border (black).
  3. Use a readable font, like Arial or [Roboto](//fonts.google.com/specimen/Roboto), in bold.
  4. Make it large enough to see without squinting.
* While Typesetting is actually quite strait-forward, doing it efficiently and well is something else entirely.
* unanimated's [Guide to Typesetting in Aegisub](//unanimated.github.io/ts/index.htm), [PDF-White](//yukisubs.files.wordpress.com/2020/04/typesetting_in_aegisub_by_unanimated_2018_white.pdf), [PDF-Black](//yukisubs.files.wordpress.com/2020/04/typesetting_in_aegisub_by_unanimated_2018_black.pdf),  [PDF-v2015](//yukisubs.files.wordpress.com/2016/10/unanimated_fansub_guides.pdf) (old). [RAR-v2015](//www.mediafire.com/file/t3zkwtzc1t33tpg/TypesettingGuide2015-03-25.rar), [RAR-v2015 mirror](//mega.nz/#F!wUYwDSgA!8tx_37HUBcs9KqPhkk5FmQ).
* unanimated's [Aegisub scripts](unanimated.github.io/ts/scripts-unanimated.htm), [PDF](//yukisubs.files.wordpress.com/2016/10/unanimated_aegisub_scripts.pdf) and [Typesetting Tools](//github.com/TypesettingTools). iamevn's [mirror](//github.com/iamevn/unanimated-Aegisub-Scripts).
* Commie's [Typesetting in Aegisub](http://commiesubs.com/interns/ts/index.htm), [PDF](//yukisubs.files.wordpress.com/2016/10/commie_typesetting_in_aegisub.pdf) and [Scripts for Aegisub - ZIP](//mega.nz/#F!wUYwDSgA!8tx_37HUBcs9KqPhkk5FmQ).
* [Mocha](//www.imagineersystems.com/products/mocha-pro), as mentioned in the guides above, can be used for motion tracking signs. A basic version of Mocha is also included natively in Adobe After Effects 11 (CS6) and newer.
* lyger's [Aegissub Automation Scripts](//github.com/lyger/Aegisub_automation_scripts).
* A short guide on [Gradients](//yukisubs.files.wordpress.com/2019/11/ongradiants-by-bloodynoyume.pdf), PDF - translated, by Bloody No Yume (French group).
* [Aegisub-Motion](//github.com/TypesettingTools/Aegisub-Motion) and [a guide](//github.com/TypesettingTools/Aegisub-Motion/wiki).
* Creative typsetting ideas: [maxfireheart.blogspot.in](//maxfireheart.blogspot.in).
* Advanced: Koby's [ASS Draw Shapes](//kametsu.com/topic/3090-ass-draw-shapes-for-subtitle-scripts) used for typesetting and KFX.
* Advanced: [Typsetting With Adobe Illustrator](//blog.line0.eu/typesetting-with-illustrator-and-ai2ass-part-i-the-basics) by Line0 and [related Blog](//blog.line0.eu).
* __Karaoke Effects (KFX):__
* Theory: This is an optional subcategory of typesetting that adds additional special effects to karaoke. Usually, KFX refers to effects beyond simple k-timing. KFX can be added to k-timed lines by applying a KFX template, modifying existing effects, or creating new effects. Some KFX can exist in softsub.ass but others must be pre-rendered (hardcoded) either because the tool to create them draws on the video stream directly, independent of k-timing, or because dynamically rendering the effect would cause severe stuttering during playback.
* As with all typesetting, applying KFX can actually be quite strait-forward, but creating and modifying new and visually appealing KFX is something else entirely. [More intro](//jockotan.wordpress.com/2015/08/12/the-basics-of-kfx).
* Prerequisite reading: 
  * How to Karaoke Templater: [1](http://docs.aegisub.org/manual/Karaoke_Templater_Tutorial_1) and [2](http://docs.aegisub.org/manual/Karaoke_Templater_Tutorial_2).
  * ["Where do I start learning?"](http://forum.aegisub.org/viewtopic.php?f=13&t=1566), [PDF](//yukisubs.files.wordpress.com/2017/09/aegisubforums-howtolearnmakingkaraoke-by-jfs.pdf) - An introduction to KFX concepts by jfs.
* Working with templates:
  * Basic: [kfx templates by ai-chan](http://forum.aegisub.org/viewtopic.php?f=13&t=1222), [ZIP - Mega](//mega.nz/#F!wUYwDSgA!8tx_37HUBcs9KqPhkk5FmQ) (subtitles-kfx).
  * Recommended: [Kara Effector](//github.com/KaraEffect0r/Kara_Effector) is a lua plugin for Aegisub that focuses on modifying provided templates. It has a lot of them and basic modifications (shapes, colors, duration, quantity) are strait-forward. Most of the documentation, [PDF](//yukisubs.files.wordpress.com/2017/05/kara-effector-usage-guide-1-39.pdf), is in Spanish.
    * Kara Effector 3.4 for Aegisub 3.2.2: [Mediafire](//www.mediafire.com/file/bbb2msh84v3y8d3/Kara+Effector+3.4+%5Bfv20.02.17%5D.rar), [Mega](//mega.nz/#F!wUYwDSgA!8tx_37HUBcs9KqPhkk5FmQ) (subtitles-kfx-Kara Effector) and the [older 3.3 version](//www.mediafire.com/file/s3y4c7m439l113w/Kara+Effector+3.3+%5Bfv24.06.16%5D.rar).
      * Kara Effector Usage Guide (1-39): Chapter PDFs available on [Mega](//mega.nz/#F!0lVXQKaJ!lOse3jVveeEqWQouBE0ekg), or see this [combined PDF (1-39)](//yukisubs.files.wordpress.com/2017/05/kara-effector-usage-guide-1-39.pdf).
      * [Youtube installation video](//www.youtube.com/watch?v=AC0YZq1tDDs), [Facebook page](//www.facebook.com/karaeffector), [Youtube homepage](//www.youtube.com/channel/UCcFmL4la4IT5HziLd9a_d7w) and some [examples](//www.youtube.com/channel/UCJWQDouAf2nxvHJwdYE-Iag).
      * Random KE formatted KFX: Mega [1](//mega.nz/#F!V9Um0JJL!uhcTl3v444RyE8gpqO8lHg) and [2, KFX_Archive_May17.zip](//mega.nz/#F!wUYwDSgA!8tx_37HUBcs9KqPhkk5FmQ) (subtitles-kfx-Kara Effector).
* Creating KFX:
  * Read this again: ["Where do I start learning?"](http://forum.aegisub.org/viewtopic.php?f=13&t=1566), [PDF](//yukisubs.files.wordpress.com/2017/09/aegisubforums-howtolearnmakingkaraoke-by-jfs.pdf) and use templates instead.
  * Very professional looking KFX can also be created using Adobe [After Effects (AE)](http://www.adobe.com/products/aftereffects.html).
  * Further reading: Aegisub's [Automation 4 Lua Overview](http://docs.aegisub.org/3.2/Automation/Lua/), some [Lua Tutorials](http://lua-users.org/wiki/TutorialDirectory) and [Programming in Lua by Roberto Ierusalimschy (3rd Edition),  PDF](//yukisubs.files.wordpress.com/2017/05/programming-in-lua-3ed.pdf).
  * Further adventures: NyuFX. [Youtube](//www.youtube.com/playlist?list=PL52E2DB0433C204F2), [SourceForge](//sourceforge.net/projects/nyufx), and [Github](//github.com/Youka/NyuFX).
  * Further adventures2: SSB. [Home thread](http://forum.aegisub.org/viewtopic.php?f=10&t=66095), [Youtube demo](//www.youtube.com/user/Youkakun/videos) and [SourceForge](//sourceforge.net/projects/ssbrenderer).

#### __Distribute (Distro)__

#### __Distro Method #1: Torrents__

* Basic: [Introduction to BitTorrent Protocol](http://bittorrent.org/introduction.html), [Beginner's Guide](//lifehacker.com/285489/a-beginners-guide-to-bittorrent), [WikiBooks](//en.wikibooks.org/wiki/The_World_of_Peer-to-Peer_%28P2P%29/Networks_and_Protocols/BitTorrent), [Wikipedia](//en.wikipedia.org/wiki/BitTorrent).

* Technical: [BitTorrent in Detail](//yukisubs.files.wordpress.com/2016/10/bittorrent_in_detail_tampere_uni_of_technology.pdf), [Specification](//wiki.theory.org/BitTorrentSpecification), and [BitTorrent Enhancement Proposals (BEPs)](http://bittorrent.org/beps/bep_0000.html).

* __Client Side__:
  
  * Recommended: [qBitTorrent](http://www.qbittorrent.org). Cross-platform cross-architecture and open source.
    * [Interesting fork](//github.com/c0re100/qBittorrent-Enhanced-Edition).
  * Windows only alternative: [uTorrent 2.2.1](http://www.oldversion.com/windows/download/utorrent-2-2-1-2) (this exact version).
    * Important: set [net.discoverable to false](//yukisubs.files.wordpress.com/2018/06/utorrent_settingschange_by_bakabt.png).
    * Interesting ruby [migration script](https://gist.github.com/naodesu/8c3c6e9bcaf81eb1f4c24b239d232736).
  * Port Forwarding: [theory](//en.wikipedia.org/wiki/Port_forwarding) and [related guide](//www.noip.com/support/knowledgebase/general-port-forwarding-guide).
  * Shana Project's [RSS Guide](https://www.shanaproject.com/help/).
  * Creating Torrent Files:
    * BakaBT's [How to create torrent files](http://wiki.bakabt.me/index.php/How_to_create_torrent_files), [PDF](//yukisubs.files.wordpress.com/2018/02/how_to_create_torrent_files_-_bakabt_wiki.pdf).       
      * For a standalone utility to create torrents, see [dottorrent-gui](//github.com/kz26/dottorrent-gui).
      * This utility also supports AnimeBytes's ["Source" property extension](//kametsu.com/topic/61665-animebytes-source-property-warning/).
      * Creating torrents faster with a CLI (advanced) [py3createtorrent](//py3createtorrent.readthedocs.io/en/latest/user.html), [DL link](//bitbucket.org/rsnitsch/py3createtorrent/downloads). 
      * Requires [Python 3.1+](//www.python.org/downloads/release) by default, but it is possible to use [pyinstaller](//pythonhosted.org/PyInstaller) to compile it into a native binary (.exe).
  * After that, upload myfile.torrent to some website. This will register it or start the registration process with the tracker if necessary. Give it a description so other peers know what you are offering.
  * For automatic torrent submission:
    * Seiya's Anidex Torrent Uploader: [Kametsu thread](//kametsu.com/topic/60527-anidex-torrent-uploader-upload-torrent-to-multiply-anime-trackers) and [Github](//github.com/seiya-dev/anidex).
    * Golumpa's [AniDexPy](https://github.com/Golumpa/AniDexPy). A simple Python tool for uploading to AniDex via its API.
  * Note: This only distributes the meta-file. For the distribution of the content, use a [seedbox](//en.wikipedia.org/wiki/Seedbox).

* __Seedbox Theory__:
  
  * [Seedboxes](//en.wikipedia.org/wiki/Seedbox) are servers that provide BitTorrent services. They can be implemented locally or rented commerically.
  * As per [Introduction to BitTorrent Protocol](http://bittorrent.org/introduction.html), any BitTorrent client-side software can potentially be used as seedbox software. 
  * Commercially, the most popular client to use for Seedbox [SaaS](//en.wikipedia.org/wiki/Software_as_a_service) offerings is [rTorrent](//github.com/rakshasa/rtorrent/wiki), [rTorrent ArchWiki](//wiki.archlinux.org/index.php/RTorrent), with the [ruTorrent](//wiki.archlinux.org/index.php/RuTorrent) frontend.
  * [Reddit/r/Seedboxes](//reddit.com/r/seedboxes).
  * For information on setting up a local seedbox please see "__Distro For Do It Yourself (DIY) People__".

* __BitTorrent Tracker Theory__:
  
  * Since backend tracker software is meant to be always active on high performance connections and require constant maintenance, it is not recommended to run one. Use existing trackers instead. However if interested, read this: [BitTorrent Tracker Theory](//esoterictek.blogspot.com/2016/10/bittorrent-tracker-theory.html).
  * There are also a number of low capacity PHP trackers designed for PHP enabled web servers and standalone tracker software executables intended to be run temporarily.

* Misc [Tutorials and Guides](//torrentinvites.org/f29/).

#### __Distro Method #2: Hyper Text Transport Protocol (HTTP) (+ Transport Layer Security (TLS))__

* __Client__:
  * [Firefox ESR](//www.mozilla.org/en-US/firefox/organizations/all) with [this](//addons.mozilla.org/en-US/firefox/addon/classicthemerestorer).
  * Firefox forks: [Palemoon](//www.palemoon.org), or [Waterfox](//www.waterfoxproject.org).
  * [Chrome](//www.google.com/chrome/browser/desktop).
  * Note: For the graphical HTTP clients above, always use [uBlock Origin](//github.com/gorhill/uBlock).
  * CLI: [Aria2c](//aria2.github.io), [wget](//www.gnu.org/software/wget) or [cURL](//curl.haxx.se/docs/manpage.html).
  * [Mega Downloader v1.7](//megadownloaderapp.blogspot.com.es/2013/01/download-links-english.html), [Mega](//mega.nz/#F!wUYwDSgA!8tx_37HUBcs9KqPhkk5FmQ). Sometimes bypasses Mega's download restrictions. SHA1 hash: D8C14D88F6C8B35FDD79CD7D208D818C4683E224
  * [JDownloader2](http://jdownloader.org/jdownloader2) Supports automatic resuming of HTTP connections (downloads) with many site-specific plugins available. Required for certain German DDL sites/forums.
* __File Server Cloud - Direct Download (DDL)__:
  * Cloud storage providers like [Mega](//Mega.nz) provide substantial but limited duration storage.
  * [Anime Tosho](//animetosho.org) mirrors the contents of English translated torrents on Nyaa and TT to cloud storage providers.
  * [Amazon](//www.amazon.com/b/?_encoding=UTF8&node=15547130011&ref_=cd_auth_home), [Google](//www.google.com/drive/pricing/), and [Microsoft](//onedrive.live.com/about/en-us/plans) provide limited long-term storage at affordable rates.
  * If you own or do not mind purchasing a domain, consider Google's [G Suite](//gsuite.google.com/features) for cost effective cloud storage.
* __Web Server Cloud__:
  * See: "Misc: The Group Blog."
* __Selfhosting (HTTP)__:
  * See "Distro: Seedboxes" and "Misc: Distro For DIY People" sections.

#### __Distro Method #3: Internet Relay Chat (IRC)__

* __Protocol Theory__: [IRC and Kludges](//esoterictek.blogspot.com/2016/10/internet-relay-chat-irc-and-kludges.html).
* __Guides__: Flash Squirrel's [How to Download using IRC](//forums.animesuki.com/showthread.php?t=3892), Kametsu's [IRC Tutorial Index](http://kametsu.com/topic/29262-tutorial-index-for-irc), and IRC client installation tutorials for [Windows](http://kametsu.com/topic/29275-installing-irc-client-on-the-windows-platform) and [OS/X](http://kametsu.com/topic/29253-irc-client-tutorial-for-the-mac).
* __Clients__: [Comparison of IRC Clients](//en.wikipedia.org/wiki/Comparison_of_Internet_Relay_Chat_clients).
  * Preferred: [Hexchat](//hexchat.github.io), previously known as "xchat", is open source, cross platform and supports limited scripting.
  * [KVIrc](http://www.kvirc.net), open source, cross platform, and astheticly pleasing. [nightly binaries](//github.com/kvirc/KVIrc/wiki/Downloading-KVIrcs-nightly-source-or-binaries).
  * [AdiRC](//www.adiirc.com), closed source freeware, cross platform, many themes available.
  * [mIRC](//www.mirc.com), proprietary and Windows only, but has powerful scripts available (e.g. to FServe). [Idiot Proof Installation Guide](//www.wikihow.com/Download-Subtitled-Japanese-Anime-from-mIRC).
  * There are also a number of web-based and mobile (iOS/Android) IRC clients that do not support DCC.
* __FServers__
  * __Client__: Keiichi's [Fserve Guide](//www.keiichianimeforever.com/guides/irc/fserv.html), [Microsoft Office Document (doc)](//yukisubs.files.wordpress.com/2016/10/introduction_to_irc_fserves_-_keiichi_anime_forever.doc), WikiBook's [Fserve Guide](//en.wikibooks.org/wiki/Downloading_Files_from_IRC/File_Server_%28fserve%29_Guide).
  * __Server__: [mIRC FServer Setup Script](//www.sysreset.com) and a [random guide](http://leonardo.spidernet.net/Copernicus/831/mirc/tips5/fserve.html).
* __XDCC__
  * __Client__: WikiBook's [Using XDCC Guide](//en.wikibooks.org/wiki/Downloading_Files_from_IRC/XDCC_Bot_Guide) and Xertion's [XDCC Commands Syntax](http://wiki.xertion.org/w/XDCC_Commands). The Xertion guide includes the syntax for batches.
  * __Server__: [XDCC Bot Guide](http://kasumi.moe/xdccguide), [PDF](//yukisubs.files.wordpress.com/2016/10/kasumi_xdcc_bot_guide.pdf),  and [iroffer-dinoex 3.3 Setup Guide](http://iroffer.dinoex.net/INSTALL-linux-en.html), [doc](//yukisubs.files.wordpress.com/2016/10/installation_-of_iroffer_mod_dinoex_under_linux_as_a_user.doc). Also: [iroffer-dinoex Homepage](http://iroffer.dinoex.de/projects/iroffer).
    * [Condensed setup guide](//gist.github.com/gdiaz384/80e0836b27a88d53dc0a9c604b972998), [iroffer-dinoex-3.30.tar.gz mirror](//mega.nz/#F!wUYwDSgA!8tx_37HUBcs9KqPhkk5FmQ) and a [Bot.config file template](http://pastebin.com/G5ZUbTCz).

#### File Transfer Protocol (FTP)

* No. This protocol needs to die. Use HTTP instead.

#### Newsgroups

* TODO: stuffs goes here.

#### __便利ツール__:

* __CRC32__: Used to put the CRC32 in brackets at the end of the filename (e.g. myfile_[1BA919D7].mkv):
  * [RapidCRC](//rapidcrc.sourceforge.net) (preferred).
  * GUI alternative: [Anime Checker](http://animechecker.sourceforge.net).
  * CLI alternative [7z h documentation](//sevenzip.osdn.jp/chm/cmdline/commands/hash.htm).
    * [bash script](//gist.github.com/Golumpa/89e3d3eeb810d7f8f539b61cffe5b29b).
* [Avdump2](//wiki.anidb.net/w/Avdump2) Based on MediaInfo. This is used to quickly update [AniDB.net](//anidb.net). See: 
  * AniDB [Wiki Tutorial](//wiki.anidb.net/w/Tutorial:How_to_Add_Files_for_Dummies!) and [Prolix Addendum](//wiki.anidb.net/w/Tutorial:How_to_Add_Files_for_Dummies!/The_Prolix_Addendum), [Mirror](//yukisubs.wordpress.com/guides/tutorial-updating-anidb-with-avdump2).
* line0's [Solutions For Taking Screenshots](//forums.bakabt.me/index.php?topic=38998.0), todo: [PDF].
* Screenshot comparison sites: 
  * [compare.bakashots.me](http://compare.bakashots.me) (only for offers on [BakaBT](//bakabt.me)).
  * [diff.pics](https://diff.pics).
  * [screenshotcomparison.com](http://screenshotcomparison.com).
* __Patches__
  * __Theory__: "Patches" are small scripts that take an existing file, a difference file (patch.vcdiff) and create a new file based on those differences. More theory: [Patches and xdelta3](//esoterictek.blogspot.com/2016/10/patches-and-xdelta3.html).
  * __Guides__:
  * moodkiller's [xdelta3 GUI](//kametsu.com/topic/56551-xdelta3-gui-20-v208-a-patch-maker-for-all/).
  * BakaBT's [Patching Guide](http://wiki.bakabt.me/index.php/Patching).
  * 13ack.Stab's [Guide to V2 Patches](http://www.animepassion.net/topic/485-guide-to-v2-patches).
  * Using patches: a simple example [FFF's Mirai Niki 7 - Patch](//mega.nz/#F!wUYwDSgA!8tx_37HUBcs9KqPhkk5FmQ) and [some complicated examples](//mega.nz/#F!Mc4zwDaQ!hJ5xLfs8GzkHqKPxNp2hLQ).
  * To create a patch:
    * CLI: xdelta3 -e 9 -s old_file new_file delta_file
    * Or [xdelta3 GUI](//osdn.net/projects/sfnet_xdelta3-gui) for GUI people. Also see: Moodkiller's [xdelta3 rebooted fork](https://github.com/Moodkiller/xdelta3-gui-2.0).
  * A binary version of xdelta3.exe can be obtained from the above patch examples or from [xdelta3 GUI](//osdn.net/projects/sfnet_xdelta3-gui).

#### __*グループ__*

* *__Theory__: Provide a way to centralize knowledge about your group including the following:*
  * *Latest release information, project archive, download options (Torrents/HTTP/XDCC/fserve), contact information (IRC/Email), community feedback mechanisms (chatbox), declared waifus, guides for the community, and donation solicitation.*
* *__Getting Started__:*
  1. *(optional) Read [The Internet and Hosting Providers](//esoterictek.blogspot.com/2016/10/the-internet-and-hosting-providers.html) to know how the internet works and how much services cost.*
  2. *(optional) Purchase a mygroup.moe domain from [Hover](//hover.com) for ~$20 (yearly). Alternative registrars: [get.moe](http://get.moe).*
  3. *Start a blog on [Blogger](//www.blogger.com) or [Wordpress](//wordpress.com).*
     * *Note: Wordpress and Weebly charge for custom domains and Blogger will disable TLS.*
  4. *Post releases. [Example](//doki.co).*
* *Markdown (formatting for blog posts):*
  * *[Markdown Cheatsheet](//github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).*
  * *[Markdown Preview](//stackedit.io/app), [v4](//stackedit.io/editor), and HTML converter.*

#### __配布をDIYするためのガイド__*

* *__General Mandatory Reading__*
  * *[The Internet and Hosting Providers](//esoterictek.blogspot.com/2016/10/the-internet-and-hosting-providers.html).*
  * *Port Forwarding [theory](//en.wikipedia.org/wiki/Port_forwarding) and [related guide](//www.noip.com/support/knowledgebase/general-port-forwarding-guide).*
  * *[Setting Up A Server](//wiki.installgentoo.com/index.php/Setting_up_a_Server) (including a [VPS](//en.wikipedia.org/wiki/Virtual_private_server)) and [Security Policy](//wiki.installgentoo.com/index.php/Setting_up_a_Server#Recommended_security_policy).*
  * *Using Crontab [Guide 1](//help.ubuntu.com/community/CronHowto) and [Guide 2](http://www.unixgeeks.org/security/newbie/unix/cron-1.html) to start tasks at startup. See: [this example](//gist.github.com/gdiaz384/343e3704dc1f955e6bd904d384566cb4).*
* *__DNS/Dynamic DNS (DDNS)__*
  * *[FreeDNS Client Update Protocol Client List](//freedns.afraid.org/scripts/freedns.clients.php), DD-WRT DDNS [Guide 1](http://www.stevejenkins.com/blog/2014/11/using-freedns-afraid-org-with-dd-wrt-when-you-lose-your-free-dyndns-or-d-link-ddns-account) and [Guide 2](//freedns.afraid.org/guide/dd-wrt/).*
  * *Namecheap's [DDNS Information](https://www.namecheap.com/support/knowledgebase/category.aspx/11/dynamic-dns) and [DDNS host guide](https://www.namecheap.com/support/knowledgebase/article.aspx/43/11/how-do-i-set-up-a-host-for-dynamic-dns).*
* *__Raspberry Pi__*
  * *[raspberryPi](//www.raspberrypi.org), [Documentation](//www.raspberrypi.org/documentation) and [Ebay Search Link](//www.ebay.com/sch/i.html?_nkw=raspberry+pi+3b%2B). *
  * *Hint: Use external storage over USB instead the Secure Digital (SD) card internal storage.*
  * *Be sure to set up [Remote Access](//www.raspberrypi.org/documentation/remote-access): [SSH](//www.raspberrypi.org/documentation/remote-access/ssh/README.md), [VNC](//www.raspberrypi.org/documentation/remote-access/vnc/README.md), (and maybe) [Samba](//www.raspberrypi.org/magpi/samba-file-server/).*
* *__Seedbox Software__*
* *[rTorrent](//wiki.archlinux.org/index.php/RTorrent) with the [ruTorrent](//wiki.archlinux.org/index.php/RuTorrent) frontend is popular due to very low resource utilization and high performance. Installations and management are usually automated:*
  * *[Quickbox](//quickbox.io), [Github](//github.com/QuickBox/QB) (recommended).*
    * *Only works for x86_64 on certain Ubuntu/Debian versions:*
  * *arakasi72's "rtinst" for Debian and Ubuntu: [Github](//github.com/arakasi72/rtinst). Note: I have not tested this.*
* *[qBittorrent](http://www.qbittorrent.org), [Wiki](//github.com/qbittorrent/qBittorrent/wiki), is cross platform and cross-architecture.*
  * *`sudo apt-get install -y qbittorrent`*
  * *Or compile it to get the latest v3.x version: See this [from scratch script](//gist.github.com/YukinoAi/1f58db68c7ef3235addbf001de44fba8). Alternatively:*
    * *[official compiling documentation](//github.com/qbittorrent/qBittorrent/wiki/Compiling-qBittorrent-on-Debian-and-Ubuntu), [arm7 compile instructions](//gist.github.com/jDmacD/9e38542901b9672728f088abd353a0a1) and [Banana seedbox](https://github.com/qbittorrent/qBittorrent/wiki/Compiling-qBittorrent-on-Raspbian-for-LeMaker-Banana-Pro). *
    * *v4.x requires QT5. [Have fun](https://wiki.qt.io/Native_Build_of_Qt_5.4.1_on_a_Raspberry_Pi).*
* *__HTTP File Server__*
  * *List of [Static HTTP Server Software](//gist.github.com/willurd/5720255).*
    * *Consider using the asynchronous "HTTP-Server" implemented using Node.js. See: [this guide](//gist.github.com/gdiaz384/94d3800fd5b3465fe7010917563581cd). *
  * *Apache and Nginx have various issues recursively auto-indexing mounted Fat32 formatted volumes via directory junctions. Just FYI~*
  * *Please no but... [HFS ~ HTTP File Server](http://www.rejetto.com/hfs) (Windows only).*
* *__TLS__*
  * *For encryption check out stunnel: [Features List](//www.stunnel.org/features.html), this [install guide](//www.digitalocean.com/community/tutorials/how-to-set-up-an-ssl-tunnel-using-stunnel-on-ubuntu).*
  * *For authentication check out [LetsEncrypt](//letsencrypt.org/docs) and the following resources: the [EFF's Certbot](//certbot.eff.org), stunnel's [LetsEncrypt configuration](//community.letsencrypt.org/t/configure-stunnel/3611) and this guide on [Configuring Cipher Suites Correctly](//weakdh.org/sysadmin.html). *
    * *Also see this TODO: [TLS combined guide].*
  * *Use SSL-Lab's [SSL Server Test](//www.ssllabs.com/ssltest) to verify the configuration once everything is set up.*

#### __最多重化__

* __Theory__: Remuxers typically focus on improving work done by other groups, combining work done by multiple groups and/or combing subs with better Audio/Visual (A/V) sources.
* __Subtitle Preprocessing Tools__:
  * Sushi's [Audio Based Subtitle Shifter](//github.com/tp7/Sushi). [Guide](//iamscum.wordpress.com/other-useful-stuff/using-sushi).
  * eXmendiC's [timing script](//iamscum.wordpress.com/auto-fixing-official-subs). Note: I have not tested this.
  * [Notepad++](//notepad-plus-plus.org). Supports "Find and Replace" across many files simultaneously.
    * [py3stringReplace](//github.com/gdiaz384/py3stringReplace). Automated version of Notepad++'s "Find and Replace".
  * Aegisub's [Timing Post Processor (TPP)](http://docs.aegisub.org/manual/Timing_Post-Processor).
  * Kageru's [snap_scenechanges.py](//gist.github.com/kageru/0e4b4f0e8b443c59552b66d5f8b55d93).
  * iamevn's [combine_lines.py](https://gist.github.com/iamevn/b21e60f6a9d572cbc5197a143f46d258).
* __Workflow__:
1. Obtain raws (See: Capping).
2. Obtain scripts.
   1. Find out which groups did the series:
      * [Anime DataBase (AniDB)](//anidb.net).
      * Search Nyaa, Anidex.moe, bakabt, etc.
        * Shortcut: [AnimeTosho](//animetosho.org)'s "Attachments" section.
      * [ar-fansub-db.blogspot.com](//ar-fansub-db.blogspot.com) and [arfansubdb.com](http://arfansubdb.com) (Arabic, Hint: Use Chrome's translation feature.).
   2. Obtain the subs or files.mkv from the group.
      * Check their website for HTTP or torrent links.
      * Check the BitTorrent tracker the group uses.
      * Check their IRC channel and look for an XDCC bot.
      * If you can find out the exact name of their files, use @find in rizon.net's #news and give it to Google.
      * Ask the group over IRC or email (unlikely to work).
      * [This one russian site](http://subs.com.ru) sometimes has scripts.
        * Use [Notepad++](//notepad-plus-plus.org/download) to change the character encoding to UTF-8 if necessary.
   3. If you can obtain the files.mkv, then stream copy or extract them out. (See: Muxing)
      * Only if hardcore: [Extracting Hardsubs](//redonesubs.blogspot.com/p/extracting-hardsubs.html), [docx](//yukisubs.files.wordpress.com/2016/10/extracting_hardsubs_-_redone_subs_-_20oct16.docx), by Zalis.
        * [Extracting Hardsubs](//jumonjigiri.blogspot.com/p/extracting-hardsubs.html) addendum by Jumonji-Giri.
      * Alternatively: [AVISubDetector](https://www.videohelp.com/software/AVISubDetector), [guide - PDF](//yukisubs.files.wordpress.com/2018/02/avisubdetector_guide_howtoripthetimingandenglishsubsfromanavifileusingavisubdetector.pdf) + [py3avi2bdnxml](https://github.com/gdiaz384/py3avi2bdnxml) + [BDSup2Sub](https://www.videohelp.com/software/BDSup2Sub) can create subtitles that [look like this](https://imgur.com/a/y7Mz2) (Czech example).
3. Fix any issues (especially syncing issues and normalization) (See: Filtering, Encoding, TLC, Editing, Timing, Typesetting).
4. Mux to preserve the changes (See: Muxing).
   * It is considered rude to use an existing groups tag in the filename, even if only minor changes were made. Use any other tag, none, a throw-away one, or your own nickname. To give them credit, label the tracks with the original source group name and credit them in any descriptions.
   * Remember to put the CRC32 in [ ] at the end of the filename (e.g. myfile_[1BA919D7].mkv). (See: Random Distro Tools for details.)
5. Distro (See: Distro).

#### *__アナログ処理__*

* *"Digital is an exercise in precision, while analog was an exercise in controlled chaos." -[digitalfaq.com](http://www.digitalfaq.com/guides/video/capture-understand-sources.htm), [Forums](http://www.digitalfaq.com/forum).*
* *__Analog Video Broadcasting History__: (fascinating btw)*
  * *Presentation slides on [Analog Communication Systems](http://slideplayer.com/slide/3990945/).*
  * *YouTube videos:*
  * *[Technology Connections](//www.youtube.com/channel/UCy0tKL1T7wFoYcxCe0xjN6Q/videos) (YouTube channel).*
    * *Before electronic television, there was [Mechanical Television](//www.youtube.com/watch?v=v5OANXk-6-w).*
    * *[Philo Farnsworth and the Invention of Electronic Television](//www.youtube.com/watch?v=NUaowcXQtOo).*
    * *[Lines of Light: How Analog Television Works](//www.youtube.com/watch?v=l4UgZBs7ZGo).*
    * *How Analog Color TV Works [The Beginnings](//www.youtube.com/watch?v=dX649lnKAU0), Part 2: [Compatible Color](//www.youtube.com/watch?v=InrDRGTPqnE) and Part 3: [more stuff](//www.youtube.com/watch?v=3JFt6t6ijLs).*
    * *[These Are Not Pixels: Revisited](//www.youtube.com/watch?v=Ea6tw-gulnQ).*
    * *[Trinitron: Sony's Once Unbeatable Product](//www.youtube.com/watch?v=0aFhzGEBQlk).*
      * *[Why is TV 29.97 frames per second?](//www.youtube.com/watch?v=3GJUM6pCpew)*
* *__Analog Decoding and Artifacting__:*
  * *An introduction to artifacts and [TV and Video Comb Filters](http://www.cockam.com/vidcomb.htm).*
  * *[Contrasting Comb Filter Types](https://www.extron.com/company/article.aspx?id=ntscdb4).*
  * *Interesting [case study](https://hometheaterhifi.com/volume_9_2/runco-pfp-11-video-processor-4-2002-part-2.html).*
  * *[Timebase Corrector (TBC) FAQ](http://www.digitalfaq.com/forum/video-restore/2251-tbc-time-base.html) and [preface](http://www.digitalfaq.com/forum/video-restore/1853-alternative-avt-8710-a.html#post9889).*
* *__Consumer Media Overview and Resources__:*
  * *Wiki on video: [Composite](//en.wikipedia.org/wiki/Composite_video), [S-Video](//en.wikipedia.org/wiki/S-Video), [Component](https://en.wikipedia.org/wiki/YPbPr). *
  * *Wiki on audio: TODO: stuff here.*
    * *[Toslink or Coax](http://thewelltemperedcomputer.com/Intro/SQ/Toslink_Coax.htm)?*
  * *Interesting [case study](//hometheaterhifi.com/volume_8_4/toshiba-sd-K700-dvd-player-12-2001.html).*
  * *__Video Home System (VHS)__: Up to 3 Mhz of analog video on magnetic tape with 240 lines of resolution.*
    * *VHS Player [User Manual Index](http://www.digitalfaq.com/forum/vcr-repair/2668-index-user-manuals.html).*
    * *YouTube videos:*
    * *[The Impossible Feat inside Your VCR](//www.youtube.com/watch?v=KfuARMCyTvg).*
    * *Why Sony's Beta Videotape System Failed: [Part 1](//www.youtube.com/watch?v=FyKRubB5N60) and [Part 2](//www.youtube.com/watch?v=v019trxfcmg).*
    * *[Comparing Beta and VHS](//www.youtube.com/watch?v=_oJs8-I9WtA).*
  * *__LaserDisc (LD)__: Up to 5 Mhz of analog video on a digital disc with 400-425 lines of resolution. Supports CD quality digital audio, and sometimes encoded AC3 or DTS.*
    * *NTSC - 262.5 lines, 59.94 Hz; PAL - 312.5 lines, 50 Hz*
    * *[Forums](http://forum.lddb.com/) and [reddit](//www.reddit.com/r/LaserDisc/). Related [library](https://yukisubs.files.wordpress.com/2018/06/antcufaalb_ld_library.jpg).*
    * *Youtube Videos:*
    * *[Laserdisc: An Introduction](//www.youtube.com/watch?v=Eg8tK1LpLS8).*
    * *[Laserdisc's Failure: What Went Wrong](//www.youtube.com/watch?v=TClRRMFZ7Sw).*
    * *[Laserdisc: Features, Follies & Evolution](//www.youtube.com/watch?v=Nbo2QepTZNY).*
    * *[DVD: The Death Knell of Laserdisc](//www.youtube.com/watch?v=cvwuAKi1ZB4).*
    * *[MUSE Hi-Vision Laserdisc: The Blu-ray of 1994](//www.youtube.com/watch?v=behaBgwnB8M).*
    * *The most boring video ever on optical media and Laserdiscs: Pioneer's  [Video Tuning Fork volume 1](//www.youtube.com/watch?v=G2HBG7HrY7s&list=PLs8mgmDyfwJfhcSCHwcb4R4V0KI0LGCGO). *
      * *Please skip this one.*
    * *[Cleaning and polishing LaserDiscs](https://www.domesday86.com/?page_id=2855).*
    * *Further viewing: Overview of the [Pioneer CLD-M301](//www.youtube.com/watch?v=L6iyUSnrGk0).*
* *__Analog Capture__: The idea is to digitize the analog audio and video signals.*
  * *Digital FAQ's [Guides Index](http://www.digitalfaq.com/guides/video.htm).*
  * *[Understanding Video Sources](http://www.digitalfaq.com/guides/video/capture-understand-sources.htm).*
  * *[Introduction to Digital Video Capturing, Recording TV](http://www.digitalfaq.com/guides/video/introduction-record-capture.htm).*
  * *VirtualDub settings guides: [Using VirtualDub to Capture AVI](http://www.digitalfaq.com/guides/video/capture-avi-virtualdub.htm) and [related discussion](http://www.digitalfaq.com/forum/video-capture/7427-capturing-virtualdub-settings.html).*
  * *Comparison of Laserdisc capture hardware via [screenshot comparisons](//originaltrilogy.com/topic/Laserdisc-players-screenshot-comparison/id/12907).*
  * *Lossless [HDMI capture comparisons](https://forum.videohelp.com/threads/376473-Lossless-HDMI-capture-devices-comparison-screenshots) (for passthrough configurations).*
  * *[__8mm__](//www.google.com/search?q=8mm+film+reels&source=lnms&tbm=isch): [Reddit wiki](//www.reddit.com/r/8mm/wiki/index).*
  * *__VHS__: *
    * *[How to Rip VHS](http://anarchivism.org/w/How_to_Rip_VHS).*
    * *[Video Hardware Suggestions; Best VCRs to Convert Tape to Digital](http://www.digitalfaq.com/guides/video/capture-playback-hardware.htm).*
  * *__LaserDisc__: *
    * *Traditional method: [How to Rip Laserdisc](http://anarchivism.org/w/How_to_Rip_Laserdisc) and [reddit topic](//www.reddit.com/r/LaserDisc/comments/3eqqhq/ripping_laserdiscs).*
    * *New method: [Doomsday Duplicator](//www.domesday86.com/?page_id=978), see [example results](//yukisubs.files.wordpress.com/2020/04/domdup_comparison.jpg). Project [background presentation](http://abug.org.uk/index.php/2020/07/04/domesday-86-part-1-the-project/?series=vabug-4th-july-2020).*
      * *Technical Background: [Hardware](//www.domesday86.com/?page_id=2233), [Software](//www.domesday86.com/?page_id=1070), [Laserdisc Decoding](https://www.domesday86.com/?page_id=1379).*
      * *[Install and Usage guide](//www.domesday86.com/?page_id=1312).*
      * *Once captured as raw, the contents must be decoded in software. Hence [ld-decode](//github.com/happycube/ld-decode/wiki) which is a "software defined LaserDisc player."*
        * *[Installation](//github.com/happycube/ld-decode/wiki/Installation), [Basic Usage Guide](https://github.com/happycube/ld-decode/wiki/Basic-usage-of-ld-decode), and [NTSC decoding](//github.com/happycube/ld-decode/wiki/Creating-video-from-NTSC-decodes) in vapoursynth.*
  * *Outdated but interesting:*
    * *[Video Workflows: Capture MPEG-2 for DVD](http://www.digitalfaq.com/guides/video/dvd-workflows-mpeg2.htm).*
    * *[Good Methods to Create DVDs (Video Workflows)](http://www.digitalfaq.com/guides/video/dvd-workflows.htm).*
