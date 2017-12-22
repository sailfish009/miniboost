minimal boost library using bcp

b2 -j8 toolset=msvc-10.0 address-model=32 architecture=x86 link=shared threading=multi runtime-link=shared --build-type=complete stage --stagedir=stage32_shared_vs2010
b2 -j8 toolset=msvc-10.0 address-model=32 architecture=x86 link=static threading=multi runtime-link=static --build-type=complete stage --stagedir=stage32_static_vs2010

b2 -j8 toolset=msvc-14.0 address-model=32 architecture=x86 link=shared threading=multi runtime-link=shared --build-type=complete stage --stagedir=stage32_shared_vs2015
b2 -j8 toolset=msvc-14.0 address-model=32 architecture=x86 link=static threading=multi runtime-link=static --build-type=complete stage --stagedir=stage32_static_vs2015