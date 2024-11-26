<p><b>CIDR notation</b> is a compact representation of an IP address and its associated network mask. The notation was invented by <a href="https://en.m.wikipedia.org/wiki/Phil_Karn" title="Phil Karn">Phil Karn</a> in the 1980s.<sup id="cite_ref-kantor_9-0" class="reference"><a href="https://en.m.wikipedia.org/wiki/Classless_Inter-Domain_Routing#cite_note-kantor-9"><span class="cite-bracket">[</span>9<span class="cite-bracket">]</span></a></sup><sup id="cite_ref-simpson_10-0" class="reference"><a href="https://en.m.wikipedia.org/wiki/Classless_Inter-Domain_Routing#cite_note-simpson-10"><span class="cite-bracket">[</span>10<span class="cite-bracket">]</span></a></sup> CIDR notation specifies an IP address, a <a href="https://en.m.wikipedia.org/wiki/Slash_(punctuation)" title="Slash (punctuation)">slash</a> ('/') character, and a decimal number. The decimal number is the count of consecutive leading <i>1</i>-bits (from left to right) in the network mask. Each 1-bit denotes a bit of the address range which must remain identical to the given IP address. The IP address in CIDR notation is always represented according to the standards for IPv4 or IPv6.
</p><p>The address may denote a specific interface address (including a host identifier, such as <i><span class="ipaddr"><span style="padding-right: 1px;">10.0.0.1</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">8</span></span></i>), or it may be the beginning address of an entire network (using a host identifier of 0, as in <i><span class="ipaddr"><span style="padding-right: 1px;">10.0.0.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">8</span></span></i> or its equivalent <i><span class="ipaddr"><span style="padding-right: 1px;">10</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">8</span></span></i>). CIDR notation can even be used with no IP address at all, e.g. when referring to a <i><span class="ipaddr"><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">24</span></span></i> as a generic description of an IPv4 network that has a 24-bit prefix and 8-bit host numbers.
</p><p>For example:
</p>
<ul><li><i><span class="ipaddr"><span style="padding-right: 1px;">198.51.100.14</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">24</span></span></i> represents the IPv4 address <i><span class="ipaddr"><span style="padding-right: 1px;">198.51.100.14</span></span></i> and its associated network prefix <i><span class="ipaddr"><span style="padding-right: 1px;">198.51.100.0</span></span></i>, or equivalently, its subnet mask <i><span class="ipaddr"><span style="padding-right: 1px;">255.255.255.0</span></span></i>, which has 24 leading <i>1</i>-bits.</li>
<li>the IPv4 block <i><span class="ipaddr"><span style="padding-right: 1px;">198.51.100.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">22</span></span></i> represents the 1024 IPv4 addresses from <i><span class="ipaddr"><span style="padding-right: 1px;">198.51.100.0</span></span></i> to <i><span class="ipaddr"><span style="padding-right: 1px;">198.51.103.255</span></span></i>.</li>
<li>the IPv6 block <i><span class="ipaddr"><span style="padding-right: 1px;">2001:db8::</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">48</span></span></i> represents the block of IPv6 addresses from <i><span class="ipaddr"><span style="padding-right: 1px;">2001:db8:0:0:0:0:0:0</span></span></i> to <i><span class="ipaddr"><span style="padding-right: 1px;">2001:db8:0:ffff:ffff:ffff:ffff:ffff</span></span></i>.</li>
<li><i><span class="ipaddr"><span style="padding-right: 1px;">::1</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">128</span></span></i> represents the IPv6 <a href="https://en.m.wikipedia.org/wiki/Loopback" title="Loopback">loopback</a> address. Its prefix length is 128 which is the number of bits in the address.</li></ul>
<p>In IPv4, CIDR notation came into wide use only after the implementation of the method, which was documented using <a href="https://en.m.wikipedia.org/wiki/Dotted-decimal" class="mw-redirect" title="Dotted-decimal">dotted-decimal</a> subnet mask specification after the slash, for example, <i><span class="ipaddr"><span style="padding-right: 1px;">192.24.12.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">255.255.252.0</span></span></i>.<sup id="cite_ref-RFC_1519_2-1" class="reference"><a href="https://en.m.wikipedia.org/wiki/Classless_Inter-Domain_Routing#cite_note-RFC_1519-2"><span class="cite-bracket">[</span>2<span class="cite-bracket">]</span></a></sup> Describing the network prefix width as a single number (<i><span class="ipaddr"><span style="padding-right: 1px;">192.24.12.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">22</span></span></i>) was easier for network administrators to conceptualize and to calculate. It became gradually incorporated into later standards documents<sup id="cite_ref-11" class="reference"><a href="https://en.m.wikipedia.org/wiki/Classless_Inter-Domain_Routing#cite_note-11"><span class="cite-bracket">[</span>11<span class="cite-bracket">]</span></a></sup><sup id="cite_ref-12" class="reference"><a href="https://en.m.wikipedia.org/wiki/Classless_Inter-Domain_Routing#cite_note-12"><span class="cite-bracket">[</span>12<span class="cite-bracket">]</span></a></sup> and into network configuration interfaces.
</p><p>The number of addresses of a network may be calculated as 2<sup>address length − prefix length</sup>, where <i>address length</i> is 128 for IPv6 and 32 for IPv4. For example, in IPv4, the prefix length <i><span class="ipaddr"><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">29</span></span></i> gives: 2<sup>32−29</sup> = 2<sup>3</sup> = 8 addresses.
</p>

---

<div class="mw-heading mw-heading3"><h3 id="IPv4_CIDR_blocks">IPv4 CIDR blocks</h3><span class="mw-editsection">
<a role="button" href="https://en.m.wikipedia.org/w/index.php?title=Classless_Inter-Domain_Routing&amp;action=edit&amp;section=6" title="Edit section: IPv4 CIDR blocks" class="cdx-button cdx-button--size-large cdx-button--fake-button cdx-button--fake-button--enabled cdx-button--icon-only cdx-button--weight-quiet ">
    <span class="minerva-icon minerva-icon--edit"></span>
<span>edit</span>
</a>

</span>

</div>
<table class="wikitable">
<tbody><tr>
<th rowspan="2">Address<br>format
</th>
<th rowspan="2">Difference<br>to last address
</th>
<th rowspan="2">Mask
</th>
<th colspan="2">Addresses
</th>
<th rowspan="2">Relative<br>to class<br>A, B, C
</th>
<th rowspan="2">Restrictions<br>on <i>a</i>, <i>b</i>, <i>c</i> and <i>d</i><br><small>(0..255 unless noted)</small>
</th>
<th rowspan="2">Typical use
</th></tr>
<tr>
<th>Decimal
</th>
<th>2<sup><i>n</i></sup>
</th></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.b.c.d</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">32</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">0.0.0.0</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.255.255.255</span></span></i>
</td>
<td style="text-align:right;">1
</td>
<td style="text-align:right;">2<sup>0</sup>
</td>
<td style="text-align:right;"><span class="frac"><span class="num">1</span>⁄<span class="den">256</span></span> C
</td>
<td>
</td>
<td>Host route
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.b.c.d</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">31</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">0.0.0.1</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.255.255.254</span></span></i>
</td>
<td style="text-align:right;">2
</td>
<td style="text-align:right;">2<sup>1</sup>
</td>
<td style="text-align:right;"><link rel="mw-deduplicated-inline-style" href="mw-data:TemplateStyles:r1154941027"><span class="frac"><span class="num">1</span>⁄<span class="den">128</span></span> C
</td>
<td><i>d</i> = 0 ... (2<i>n</i>) ... 254
</td>
<td>Point-to-point links (<link rel="mw-deduplicated-inline-style" href="mw-data:TemplateStyles:r1238218222"><a href="https://en.m.wikipedia.org/wiki/RFC_(identifier)" class="mw-redirect" title="RFC (identifier)">RFC</a>&nbsp;<a rel="nofollow" class="external text" href="https://datatracker.ietf.org/doc/html/rfc3021">3021</a>)
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.b.c.d</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">30</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">0.0.0.3</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.255.255.252</span></span></i>
</td>
<td style="text-align:right;">4
</td>
<td style="text-align:right;">2<sup>2</sup>
</td>
<td style="text-align:right;"><link rel="mw-deduplicated-inline-style" href="mw-data:TemplateStyles:r1154941027"><span class="frac"><span class="num">1</span>⁄<span class="den">64</span></span> C
</td>
<td><i>d</i> = 0 ... (4<i>n</i>) ... 252
</td>
<td><span class="nowrap">Point-to-point links (glue network)</span>
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.b.c.d</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">29</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">0.0.0.7</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.255.255.248</span></span></i>
</td>
<td style="text-align:right;">8
</td>
<td style="text-align:right;">2<sup>3</sup>
</td>
<td style="text-align:right;"><link rel="mw-deduplicated-inline-style" href="mw-data:TemplateStyles:r1154941027"><span class="frac"><span class="num">1</span>⁄<span class="den">32</span></span> C
</td>
<td><i>d</i> = 0 ... (8<i>n</i>) ... 248
</td>
<td>Smallest multi-host network
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.b.c.d</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">28</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">0.0.0.15</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.255.255.240</span></span></i>
</td>
<td style="text-align:right;">16
</td>
<td style="text-align:right;">2<sup>4</sup>
</td>
<td style="text-align:right;"><link rel="mw-deduplicated-inline-style" href="mw-data:TemplateStyles:r1154941027"><span class="frac"><span class="num">1</span>⁄<span class="den">16</span></span> C
</td>
<td><i>d</i> = 0 ... (16<i>n</i>) ... 240
</td>
<td rowspan="3">Small <a href="https://en.m.wikipedia.org/wiki/LAN" class="mw-redirect" title="LAN">LAN</a>
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.b.c.d</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">27</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">0.0.0.31</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.255.255.224</span></span></i>
</td>
<td style="text-align:right;">32
</td>
<td style="text-align:right;">2<sup>5</sup>
</td>
<td style="text-align:right;"><link rel="mw-deduplicated-inline-style" href="mw-data:TemplateStyles:r1154941027"><span class="frac"><span class="num">1</span>⁄<span class="den">8</span></span> C
</td>
<td><i>d</i> = 0 ... (32<i>n</i>) ... 224
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.b.c.d</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">26</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">0.0.0.63</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.255.255.192</span></span></i>
</td>
<td style="text-align:right;">64
</td>
<td style="text-align:right;">2<sup>6</sup>
</td>
<td style="text-align:right;"><link rel="mw-deduplicated-inline-style" href="mw-data:TemplateStyles:r1154941027"><span class="frac"><span class="num">1</span>⁄<span class="den">4</span></span> C
</td>
<td><i>d</i> = 0, 64, 128, 192
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.b.c.d</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">25</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">0.0.0.127</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.255.255.128</span></span></i>
</td>
<td style="text-align:right;">128
</td>
<td style="text-align:right;">2<sup>7</sup>
</td>
<td style="text-align:right;"><link rel="mw-deduplicated-inline-style" href="mw-data:TemplateStyles:r1154941027"><span class="frac"><span class="num">1</span>⁄<span class="den">2</span></span> C
</td>
<td><i>d</i> = 0, 128
</td>
<td rowspan="2">Large <a href="https://en.m.wikipedia.org/wiki/LAN" class="mw-redirect" title="LAN">LAN</a>
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.b.c.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">24</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">0.0.0.255</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.255.255.0</span></span></i>
</td>
<td style="text-align:right;">256
</td>
<td style="text-align:right;">2<sup>8</sup>
</td>
<td style="text-align:right;">1 C
</td>
<td>
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.b.c.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">23</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">0.0.1.255</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.255.254.0</span></span></i>
</td>
<td style="text-align:right;">512
</td>
<td style="text-align:right;">2<sup>9</sup>
</td>
<td style="text-align:right;">2 C
</td>
<td><i>c</i> = 0 ... (2<i>n</i>) ... 254
</td>
<td>
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.b.c.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">22</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">0.0.3.255</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.255.252.0</span></span></i>
</td>
<td style="text-align:right;">1,024
</td>
<td style="text-align:right;">2<sup>10</sup>
</td>
<td style="text-align:right;">4 C
</td>
<td><i>c</i> = 0 ... (4<i>n</i>) ... 252
</td>
<td>Small business
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.b.c.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">21</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">0.0.7.255</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.255.248.0</span></span></i>
</td>
<td style="text-align:right;">2,048
</td>
<td style="text-align:right;">2<sup>11</sup>
</td>
<td style="text-align:right;">8 C
</td>
<td><i>c</i> = 0 ... (8<i>n</i>) ... 248
</td>
<td rowspan="2">Small <a href="https://en.m.wikipedia.org/wiki/ISP" class="mw-redirect" title="ISP">ISP</a>/ large business
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.b.c.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">20</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">0.0.15.255</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.255.240.0</span></span></i>
</td>
<td style="text-align:right;">4,096
</td>
<td style="text-align:right;">2<sup>12</sup>
</td>
<td style="text-align:right;">16 C
</td>
<td><i>c</i> = 0 ... (16<i>n</i>) ... 240
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.b.c.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">19</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">0.0.31.255</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.255.224.0</span></span></i>
</td>
<td style="text-align:right;">8,192
</td>
<td style="text-align:right;">2<sup>13</sup>
</td>
<td style="text-align:right;">32 C
</td>
<td><i>c</i> = 0 ... (32<i>n</i>) ... 224
</td>
<td rowspan="3"><a href="https://en.m.wikipedia.org/wiki/ISP" class="mw-redirect" title="ISP">ISP</a>/ large business
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.b.c.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">18</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">0.0.63.255</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.255.192.0</span></span></i>
</td>
<td style="text-align:right;">16,384
</td>
<td style="text-align:right;">2<sup>14</sup>
</td>
<td style="text-align:right;">64 C
</td>
<td><i>c</i> = 0, 64, 128, 192
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.b.c.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">17</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">0.0.127.255</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.255.128.0</span></span></i>
</td>
<td style="text-align:right;">32,768
</td>
<td style="text-align:right;">2<sup>15</sup>
</td>
<td style="text-align:right;">128 C
</td>
<td><i>c</i> = 0, 128
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.b.0.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">16</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">0.0.255.255</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.255.0.0</span></span></i>
</td>
<td style="text-align:right;">65,536
</td>
<td style="text-align:right;">2<sup>16</sup>
</td>
<td style="text-align:right;">256 C = B
</td>
<td>
</td>
<td>
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.b.0.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">15</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">0.1.255.255</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.254.0.0</span></span></i>
</td>
<td style="text-align:right;">131,072
</td>
<td style="text-align:right;">2<sup>17</sup>
</td>
<td style="text-align:right;">2 B
</td>
<td><i>b</i> = 0 ... (2<i>n</i>) ... 254
</td>
<td>
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.b.0.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">14</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">0.3.255.255</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.252.0.0</span></span></i>
</td>
<td style="text-align:right;">262,144
</td>
<td style="text-align:right;">2<sup>18</sup>
</td>
<td style="text-align:right;">4 B
</td>
<td><i>b</i> = 0 ... (4<i>n</i>) ... 252
</td>
<td>
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.b.0.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">13</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">0.7.255.255</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.248.0.0</span></span></i>
</td>
<td style="text-align:right;">524,288
</td>
<td style="text-align:right;">2<sup>19</sup>
</td>
<td style="text-align:right;">8 B
</td>
<td><i>b</i> = 0 ... (8<i>n</i>) ... 248
</td>
<td>
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.b.0.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">12</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">0.15.255.255</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.240.0.0</span></span></i>
</td>
<td style="text-align:right;">1,048,576
</td>
<td style="text-align:right;">2<sup>20</sup>
</td>
<td style="text-align:right;">16 B
</td>
<td><i>b</i> = 0 ... (16<i>n</i>) ... 240
</td>
<td>
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.b.0.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">11</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">0.31.255.255</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.224.0.0</span></span></i>
</td>
<td style="text-align:right;">2,097,152
</td>
<td style="text-align:right;">2<sup>21</sup>
</td>
<td style="text-align:right;">32 B
</td>
<td><i>b</i> = 0 ... (32<i>n</i>) ... 224
</td>
<td>
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.b.0.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">10</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">0.63.255.255</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.192.0.0</span></span></i>
</td>
<td style="text-align:right;">4,194,304
</td>
<td style="text-align:right;">2<sup>22</sup>
</td>
<td style="text-align:right;">64 B
</td>
<td><i>b</i> = 0, 64, 128, 192
</td>
<td>
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.b.0.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">9</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">0.127.255.255</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.128.0.0</span></span></i>
</td>
<td style="text-align:right;">8,388,608
</td>
<td style="text-align:right;">2<sup>23</sup>
</td>
<td style="text-align:right;">128 B
</td>
<td><i>b</i> = 0, 128
</td>
<td>
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.0.0.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">8</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">0.255.255.255</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.0.0.0</span></span></i>
</td>
<td style="text-align:right;">16,777,216
</td>
<td style="text-align:right;">2<sup>24</sup>
</td>
<td style="text-align:right;">256 B = A
</td>
<td>
</td>
<td>Largest <a href="https://en.m.wikipedia.org/wiki/IANA" class="mw-redirect" title="IANA">IANA</a> block allocation
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.0.0.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">7</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">1.255.255.255</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">254.0.0.0</span></span></i>
</td>
<td style="text-align:right;">33,554,432
</td>
<td style="text-align:right;">2<sup>25</sup>
</td>
<td style="text-align:right;">2 A
</td>
<td><i>a</i> = 0 ... (2<i>n</i>) ... 254
</td>
<td>
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.0.0.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">6</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">3.255.255.255</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">252.0.0.0</span></span></i>
</td>
<td style="text-align:right;">67,108,864
</td>
<td style="text-align:right;">2<sup>26</sup>
</td>
<td style="text-align:right;">4 A
</td>
<td><i>a</i> = 0 ... (4<i>n</i>) ... 252
</td>
<td>
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.0.0.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">5</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">7.255.255.255</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">248.0.0.0</span></span></i>
</td>
<td style="text-align:right;">134,217,728
</td>
<td style="text-align:right;">2<sup>27</sup>
</td>
<td style="text-align:right;">8 A
</td>
<td><i>a</i> = 0 ... (8<i>n</i>) ... 248
</td>
<td>
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.0.0.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">4</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">15.255.255.255</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">240.0.0.0</span></span></i>
</td>
<td style="text-align:right;">268,435,456
</td>
<td style="text-align:right;">2<sup>28</sup>
</td>
<td style="text-align:right;">16 A
</td>
<td><i>a</i> = 0 ... (16<i>n</i>) ... 240
</td>
<td>
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.0.0.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">3</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">31.255.255.255</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">224.0.0.0</span></span></i>
</td>
<td style="text-align:right;">536,870,912
</td>
<td style="text-align:right;">2<sup>29</sup>
</td>
<td style="text-align:right;">32 A
</td>
<td><i>a</i> = 0 ... (32<i>n</i>) ... 224
</td>
<td>
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.0.0.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">2</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">63.255.255.255</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">192.0.0.0</span></span></i>
</td>
<td style="text-align:right;">1,073,741,824
</td>
<td style="text-align:right;">2<sup>30</sup>
</td>
<td style="text-align:right;">64 A
</td>
<td><i>a</i> = 0, 64, 128, 192
</td>
<td>
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">a.0.0.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">1</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">127.255.255.255</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">128.0.0.0</span></span></i>
</td>
<td style="text-align:right;">2,147,483,648
</td>
<td style="text-align:right;">2<sup>31</sup>
</td>
<td style="text-align:right;">128 A
</td>
<td><i>a</i> = 0, 128
</td>
<td>
</td></tr>
<tr>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">0.0.0.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">0</span></span></i>
</td>
<td>+<i><span class="ipaddr"><span style="padding-right: 1px;">255.255.255.255</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">0.0.0.0</span></span></i>
</td>
<td style="text-align:right;">4,294,967,296
</td>
<td style="text-align:right;">2<sup>32</sup>
</td>
<td style="text-align:right;">256 A
</td>
<td>
</td>
<td>Entire IPv4 Internet, <a href="https://en.m.wikipedia.org/wiki/Default_route" title="Default route">default route</a>.
</td></tr></tbody></table>
<p>In common usage, the first address in a subnet, all binary zero in the host identifier, is reserved for referring to the network itself, while the last address, all binary one in the host identifier, is used as a <a href="https://en.m.wikipedia.org/wiki/Broadcast_address" title="Broadcast address">broadcast address</a> for the network; this reduces the number of addresses available for hosts by 2. As a result, a <i><span class="ipaddr"><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">31</span></span></i> network, with one binary digit in the host identifier, would be unusable, as such a subnet would provide no available host addresses after this reduction. <link rel="mw-deduplicated-inline-style" href="mw-data:TemplateStyles:r1238218222"><a href="https://en.m.wikipedia.org/wiki/RFC_(identifier)" class="mw-redirect" title="RFC (identifier)">RFC</a>&nbsp;<a rel="nofollow" class="external text" href="https://datatracker.ietf.org/doc/html/rfc3021">3021</a> creates an exception to the "host all ones" and "host all zeros" rules to make <i><span class="ipaddr"><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">31</span></span></i> networks usable for point-to-point links. <i><span class="ipaddr"><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">32</span></span></i> addresses (single-host network) must be accessed by explicit routing rules, as there is no room in such a network for a gateway.
</p><p>In routed subnets larger than <i><span class="ipaddr"><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">31</span></span></i> or <i><span class="ipaddr"><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">32</span></span></i>, the number of available host addresses is usually reduced by two, namely the largest address, which is reserved as the broadcast address, and the smallest address, which identifies the network itself.<sup id="cite_ref-RFC_922_15-0" class="reference"><a href="https://en.m.wikipedia.org/wiki/Classless_Inter-Domain_Routing#cite_note-RFC_922-15"><span class="cite-bracket">[</span>15<span class="cite-bracket">]</span></a></sup><sup id="cite_ref-RFC_1812_16-0" class="reference"><a href="https://en.m.wikipedia.org/wiki/Classless_Inter-Domain_Routing#cite_note-RFC_1812-16"><span class="cite-bracket">[</span>16<span class="cite-bracket">]</span></a></sup>
</p>

在常见用法中，子网中的第一个地址（主机标识符中全为二进制零）被保留用于引用网络本身，而最后一个地址（主机标识符中全为二进制一）被用作网络的广播地址；这将主机可用的地址数减少了 **2** 。因此，主机标识符中只有一位二进制数字的 **/31** 网络将无法使用，因为这样的子网在减少后将不会提供可用的主机地址。RFC3021对*主机全一*和*主机全零*规则创建了一个例外，以使 **/31** 网络可用于点对点链接。**/32** 地址（单主机网络）必须通过显式路由规则访问，因为这样的网络中没有网关的空间。

在大于 **/31** 或 **/32** 的路由子网中，可用主机地址的数量通常减少两个，即最大的地址（保留为广播地址）和最小的地址（标识网络本身）。[15][16]
