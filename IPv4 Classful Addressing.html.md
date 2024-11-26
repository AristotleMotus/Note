<dl><dt>Classes</dt></dl>
<table class="wikitable">
<tbody><tr>
<th>Class
</th>
<th>Leading bits
</th>
<th>Size of <i>network number</i> bit field
</th>
<th>Size of <i>rest</i> bit field
</th>
<th>Number of networks
</th>
<th>Addresses per network
</th>
<th>Total addresses in class
</th>
<th>Start address
</th>
<th>End address
</th>
<th>Default <a href="https://en.m.wikipedia.org/wiki/Subnet_mask" class="mw-redirect" title="Subnet mask">subnet mask</a> in <a href="https://en.m.wikipedia.org/wiki/Dot-decimal_notation" title="Dot-decimal notation">dot-decimal notation</a>
</th>
<th><a href="https://en.m.wikipedia.org/wiki/CIDR_notation" class="mw-redirect" title="CIDR notation">CIDR notation</a>
</th></tr>
<tr>
<td>Class A
</td>
<td>0
</td>
<td>8
</td>
<td>24
</td>
<td>128 (2<sup>7</sup>)
</td>
<td>16,777,216 (2<sup>24</sup>)
</td>
<td>2,147,483,648 (2<sup>31</sup>)
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">0.0.0.0</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">127.255.255.255</span></span></i><sup id="cite_ref-7" class="reference"><a href="https://en.m.wikipedia.org/wiki/Classful_network#cite_note-7"><span class="cite-bracket">[</span>a<span class="cite-bracket">]</span></a></sup>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.0.0.0</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">8</span></span></i>
</td></tr>
<tr>
<td>Class B
</td>
<td>10
</td>
<td>16
</td>
<td>16
</td>
<td>16,384 (2<sup>14</sup>)
</td>
<td>65,536 (2<sup>16</sup>)
</td>
<td>1,073,741,824 (2<sup>30</sup>)
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">128.0.0.0</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">191.255.255.255</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.255.0.0</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">16</span></span></i>
</td></tr>
<tr>
<td>Class C
</td>
<td>110
</td>
<td>24
</td>
<td>8
</td>
<td>2,097,152 (2<sup>21</sup>)
</td>
<td>256 (2<sup>8</sup>)
</td>
<td>536,870,912 (2<sup>29</sup>)
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">192.0.0.0</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">223.255.255.255</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.255.255.0</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">24</span></span></i>
</td></tr>
<tr>
<td>Class D (<a href="https://en.m.wikipedia.org/wiki/Multicast" title="Multicast">multicast</a>)
</td>
<td>1110
</td>
<td>not defined
</td>
<td>not defined
</td>
<td>not defined
</td>
<td>not defined
</td>
<td>268,435,456 (2<sup>28</sup>)
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">224.0.0.0</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">239.255.255.255</span></span></i>
</td>
<td>not defined
</td>
<td>/4<sup id="cite_ref-8" class="reference"><a href="https://en.m.wikipedia.org/wiki/Classful_network#cite_note-8"><span class="cite-bracket">[</span>7<span class="cite-bracket">]</span></a></sup>
</td></tr>
<tr>
<td>Class E (reserved)
</td>
<td>1111
</td>
<td>not defined
</td>
<td>not defined
</td>
<td>not defined
</td>
<td>not defined
</td>
<td>268,435,456 (2<sup>28</sup>)
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">240.0.0.0</span></span></i>
</td>
<td><i><span class="ipaddr"><span style="padding-right: 1px;">255.255.255.255</span></span></i><sup id="cite_ref-9" class="reference"><a href="https://en.m.wikipedia.org/wiki/Classful_network#cite_note-9"><span class="cite-bracket">[</span>b<span class="cite-bracket">]</span></a></sup>
</td>
<td>not defined
</td>
<td>not defined
</td></tr></tbody></table>

---

<dl><dt>Bit-wise representation</dt></dl>
<p>In the following bit-wise representation,
</p>
<ul><li><i>n</i> indicates a bit used for the network ID.</li>
<li><i>H</i> indicates a bit used for the host ID.</li>
<li><i>X</i> indicates a bit without a specified purpose.</li></ul>
<pre>Class A
  0.  0.  0.  0 = 00000000.00000000.00000000.00000000
127.255.255.255 = 01111111.11111111.11111111.11111111
                  0nnnnnnn.HHHHHHHH.HHHHHHHH.HHHHHHHH

Class B
128.  0.  0.  0 = 10000000.00000000.00000000.00000000
191.255.255.255 = 10111111.11111111.11111111.11111111
                  10nnnnnn.nnnnnnnn.HHHHHHHH.HHHHHHHH

Class C
192.  0.  0.  0 = 11000000.00000000.00000000.00000000
223.255.255.255 = 11011111.11111111.11111111.11111111
                  110nnnnn.nnnnnnnn.nnnnnnnn.HHHHHHHH

Class D
224.  0.  0.  0 = 11100000.00000000.00000000.00000000
239.255.255.255 = 11101111.11111111.11111111.11111111
                  1110XXXX.XXXXXXXX.XXXXXXXX.XXXXXXXX

Class E
240.  0.  0.  0 = 11110000.00000000.00000000.00000000
255.255.255.255 = 11111111.11111111.11111111.11111111
                  1111XXXX.XXXXXXXX.XXXXXXXX.XXXXXXXX
</pre>

---

<p>The number of addresses usable for addressing specific hosts in each network is always <span class="nowrap">2<sup>N</sup> - 2</span>, where N is the number of rest field bits, and the subtraction of 2 adjusts for the use of the all-bits-zero host value to represent the network address and the all-bits-one host value for use as a broadcast address. Thus, for a Class C address with 8 bits available in the host field, the maximum number of hosts is 254.
</p><p>Today, IP addresses are associated with a <a href="https://en.m.wikipedia.org/wiki/Subnet_mask" class="mw-redirect" title="Subnet mask">subnet mask</a>. This was not required in a classful network because the mask was implied by the address itself; any network device would inspect the first few bits of the IP address to determine the class of the address and thus its netmask.
</p><p>The blocks numerically at the start and end of classes A, B and C were originally reserved for special addressing or future features, i.e., <i><span class="ipaddr"><span style="padding-right: 1px;">0.0.0.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">8</span></span></i> and <i><span class="ipaddr"><span style="padding-right: 1px;">127.0.0.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">8</span></span></i> are reserved in former class A; <i><span class="ipaddr"><span style="padding-right: 1px;">128.0.0.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">16</span></span></i> and <i><span class="ipaddr"><span style="padding-right: 1px;">191.255.0.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">16</span></span></i> were reserved in former class B but are now available for assignment; <i><span class="ipaddr"><span style="padding-right: 1px;">192.0.0.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">24</span></span></i> and <i><span class="ipaddr"><span style="padding-right: 1px;">223.255.255.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">24</span></span></i> are reserved in former class C. While the <i><span class="ipaddr"><span style="padding-right: 1px;">127.0.0.0</span><span style="padding-right: 1px;">/</span><span style="padding-right: 1px;">8</span></span></i> network is a Class A network, it is designated for <a href="https://en.m.wikipedia.org/wiki/Loopback" title="Loopback">loopback</a> and cannot be assigned to a network.<sup id="cite_ref-RFC_5735_10-0" class="reference"><a href="https://en.m.wikipedia.org/wiki/Classful_network#cite_note-RFC_5735-10"><span class="cite-bracket">[</span>8<span class="cite-bracket">]</span></a></sup>
</p><p>Class D is reserved for <a href="https://en.m.wikipedia.org/wiki/Multicast" title="Multicast">multicast</a> and cannot be used for regular unicast traffic. Class E is reserved and cannot be used on the public Internet. Many older routers will not accept using it in any context.<sup class="noprint Inline-Template Template-Fact" style="white-space:nowrap;">[<i><a href="https://en.m.wikipedia.org/wiki/Wikipedia:Citation_needed" title="Wikipedia:Citation needed"><span title="This claim needs references to reliable sources. (July 2018)">citation needed</span></a></i>]</sup>
</p>
