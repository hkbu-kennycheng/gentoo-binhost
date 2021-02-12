# x86_64-pc-linux-gnu


Packages optimized for Generic x86_64 AMD/Intel Processors.

<img src="https://raw.githubusercontent.com/ahnafhabib404/gentoo-binhost/master/images/648625-vermeer-black-chip-render-1260x709_2.png" alt="648625-vermeer-black-chip-render-1260x709_2" width="250" />



Example (AMD FX 8350)

```
$ lscpu
Architecture:                    x86_64
CPU op-mode(s):                  32-bit, 64-bit
Byte Order:                      Little Endian
Address sizes:                   48 bits physical, 48 bits virtual
CPU(s):                          8
On-line CPU(s) list:             0-7
Thread(s) per core:              2
Core(s) per socket:              4
Socket(s):                       1
NUMA node(s):                    1
Vendor ID:                       AuthenticAMD
CPU family:                      21
Model:                           2
Model name:                      AMD FX(tm)-8350 Eight-Core Processor
Stepping:                        0
Frequency boost:                 enabled
CPU MHz:                         2096.815
CPU max MHz:                     4000.0000
CPU min MHz:                     1400.0000
BogoMIPS:                        8003.06
Virtualization:                  AMD-V
L1d cache:                       64 KiB
L1i cache:                       256 KiB
L2 cache:                        8 MiB
L3 cache:                        8 MiB
NUMA node0 CPU(s):               0-7
Vulnerability Itlb multihit:     Not affected
Vulnerability L1tf:              Not affected
Vulnerability Mds:               Not affected
Vulnerability Meltdown:          Not affected
Vulnerability Spec store bypass: Mitigation; Speculative Store Bypass disabled via prctl and seccomp
Vulnerability Spectre v1:        Mitigation; usercopy/swapgs barriers and __user pointer sanitization
Vulnerability Spectre v2:        Mitigation; Full AMD retpoline, IBPB conditional, STIBP disabled, RSB filling
Vulnerability Srbds:             Not affected
Vulnerability Tsx async abort:   Not affected
Flags:                           fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fx
                                 sr sse sse2 ht syscall nx mmxext fxsr_opt pdpe1gb rdtscp lm constant_tsc rep_good nopl
                                  nonstop_tsc cpuid extd_apicid aperfmperf pni pclmulqdq monitor ssse3 fma cx16 sse4_1 
                                 sse4_2 popcnt aes xsave avx f16c lahf_lm cmp_legacy svm extapic cr8_legacy abm sse4a m
                                 isalignsse 3dnowprefetch osvw ibs xop skinit wdt fma4 tce nodeid_msr tbm topoext perfc
                                 tr_core perfctr_nb cpb hw_pstate ssbd ibpb vmmcall bmi1 arat npt lbrv svm_lock nrip_sa
                                 ve tsc_scale vmcb_clean flushbyasid decodeassists pausefilter pfthreshold
```
## Usage

Binhost can be enabled by adding these lines to the **make.conf**.

```bash
# enable binhost
PORTAGE_BINHOST="https://raw.githubusercontent.com/ahnafhabib404/gentoo-binhost/${CHOST}"
FEATURES="${FEATURES} getbinpkg"
```

## Details

### Profile

Packages are generated using gentoo 17.1 desktop profile.

USE Flags
```
USE="X a52 aac acl acpi alsa amd64 berkdb bindist bluetooth branding bzip2 cairo cdda cdr cli crypt cups dbus dri dts dvd dvdr elogind emboss encode exif flac fortran gdbm gif gpm gtk gui iconv icu ipv6 jpeg lcms libglvnd libnotify libtirpc mad mng mp3 mp4 mpeg multilib ncurses networkmanager nls nptl ogg opengl openmp pam pango pcre pdf png policykit ppds pulseaudio qt5 readline sdl seccomp spell split-usr ssl startup-notification svg tcpd tiff truetype udev udisks unicode upower usb vorbis wifi wxwidgets x264 xattr xcb xml xv xvid zlib" ABI_X86="64" ADA_TARGET="gnat_2018" ALSA_CARDS="ali5451 als4000 atiixp atiixp-modem bt87x ca0106 cmipci emu10k1x ens1370 ens1371 es1938 es1968 fm801 hda-intel intel8x0 intel8x0m maestro3 trident usb-audio via82xx via82xx-modem ymfpci" APACHE2_MODULES="authn_core authz_core socache_shmcb unixd actions alias auth_basic authn_alias authn_anon authn_dbm authn_default authn_file authz_dbm authz_default authz_groupfile authz_host authz_owner authz_user autoindex cache cgi cgid dav dav_fs dav_lock deflate dir disk_cache env expires ext_filter file_cache filter headers include info log_config logio mem_cache mime mime_magic negotiation rewrite setenvif speling status unique_id userdir usertrack vhost_alias" CALLIGRA_FEATURES="karbon sheets words" COLLECTD_PLUGINS="df interface irq load memory rrdtool swap syslog" CPU_FLAGS_X86="aes avx f16c fma3 fma4 mmx mmxext pclmul popcnt sse sse2 sse3 sse4_1 sse4_2 sse4a ssse3 xop" ELIBC="glibc" GPSD_PROTOCOLS="ashtech aivdm earthmate evermore fv18 garmin garmintxt gpsclock greis isync itrax mtk3301 nmea ntrip navcom oceanserver oldstyle oncore rtcm104v2 rtcm104v3 sirf skytraq superstar2 timing tsip tripmate tnt ublox ubx" INPUT_DEVICES="libinput" KERNEL="linux" LCD_DEVICES="bayrad cfontz cfontz633 glk hd44780 lb216 lcdm001 mtxorb ncurses text" LIBREOFFICE_EXTENSIONS="presenter-console presenter-minimizer" LUA_SINGLE_TARGET="lua5-1" LUA_TARGETS="lua5-1" OFFICE_IMPLEMENTATION="libreoffice" PHP_TARGETS="php7-3 php7-4" POSTGRES_TARGETS="postgres10 postgres11" PYTHON_SINGLE_TARGET="python3_8" PYTHON_TARGETS="python3_8" RUBY_TARGETS="ruby26" USERLAND="GNU" VIDEO_CARDS="amdgpu fbdev intel nouveau radeon radeonsi vesa dummy v4l" XTABLES_ADDONS="quota2 psd pknock lscan length2 ipv4options ipset ipp2p iface geoip fuzzy condition tee tarpit sysrq steal rawnat logmark ipmark dhcpmac delude chaos account"
```
C FLAGS
```
COMMON_FLAGS=" -march=native -O2 -pipe"
CFLAGS="${COMMON_FLAGS}"
CXXFLAGS="${COMMON_FLAGS}"
FCFLAGS="${COMMON_FLAGS}"
FFLAGS="${COMMON_FLAGS}"
```
