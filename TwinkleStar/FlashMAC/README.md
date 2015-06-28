Introduction
===

If you want to write MAC, you must ensure that mtd factory is writable.
Remove the factory's read-only properties in the TwinkleStar.dts.
	
vim TwinkleStar.dts

......

	factory: partition@40000 {

		label = "factory";

		reg = <0x40000 0x10000>;

		#read-only;

	};

......

Download Twinklestarmacjsonp.html and How to flash the MAC via the web.doc
