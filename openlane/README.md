# OpenLane Template

这个是openlane模版的测试项目

使用方法：
1. `git clone https://github.com/poorjobless/openlane-template-gcd`
2. `cd openlane-template-gcd/openlane`
3. `make`

如果最后提示 [SUCCESS]: Flow Completed Without Fatal Errors.
表示RTL to GDSII生成成功，你的环境是正常的。此时版图文件位于你的项目根目录下的gds文件夹里。

生成成功后的目录结构
.
├── def
│   └── gcd.def
├── gds
│   └── gcd.gds
├── lef
│   └── gcd.lef
├── mag
│   └── gcd.mag
├── maglef
│   └── gcd.mag
├── openlane
│   ├── .bashrc
│   ├── .zshrc
│   ├── default.cvcrc
│   ├── dependencies
│   │   ├── tool_metadata.yml
│   │   └── tool.py
│   ├── gcd
│   │   ├── base.sdc
│   │   ├── config.tcl
│   │   ├── interactive.tcl0
│   │   ├── pdn.tcl
│   │   ├── pin_order.cfg
│   │   ├── runs
│   │   │   └── gcd
│   │   │       ├── cmds.log
│   │   │       ├── config.tcl
│   │   │       ├── logs
│   │   │       │   ├── 0-prep_runtime.txt
│   │   │       │   ├── 10-write_verilog.log
│   │   │       │   ├── 10-write_verilog_runtime.txt
│   │   │       │   ├── 15-write_verilog.log
│   │   │       │   ├── 15-write_verilog_runtime.txt
│   │   │       │   ├── 19-write_verilog.log
│   │   │       │   ├── 19-write_verilog_runtime.txt
│   │   │       │   ├── 25-write_verilog.log
│   │   │       │   ├── 25-write_verilog_runtime.txt
│   │   │       │   ├── cts
│   │   │       │   │   ├── 14-cts.log
│   │   │       │   │   └── 14-cts_runtime.txt
│   │   │       │   ├── cvc
│   │   │       │   │   ├── 42-cvc_runtime.txt
│   │   │       │   │   └── 42-cvc_screen.log
│   │   │       │   ├── floorplan
│   │   │       │   │   ├── 3-verilog2def.openroad.log
│   │   │       │   │   ├── 3-verilog2def_openroad_runtime.txt
│   │   │       │   │   ├── 4-place_io_ol.log
│   │   │       │   │   ├── 5-tapcell.log
│   │   │       │   │   ├── 5-tapcell_runtime.txt
│   │   │       │   │   ├── 7-pdn.log
│   │   │       │   │   └── 7-pdn_runtime.txt
│   │   │       │   ├── flow_summary.log
│   │   │       │   ├── klayout
│   │   │       │   │   ├── 13-klayout.scrot.log
│   │   │       │   │   ├── 13-klayout_scrot_runtime.txt
│   │   │       │   │   ├── 16-klayout.scrot.log
│   │   │       │   │   ├── 16-klayout_scrot_runtime.txt
│   │   │       │   │   ├── 21-klayout.scrot.log
│   │   │       │   │   ├── 21-klayout_scrot_runtime.txt
│   │   │       │   │   ├── 27-klayout.scrot.log
│   │   │       │   │   ├── 27-klayout_scrot_runtime.txt
│   │   │       │   │   ├── 31-klayout.log
│   │   │       │   │   ├── 31-klayout_runtime.txt
│   │   │       │   │   ├── 32-klayout.scrot.log
│   │   │       │   │   ├── 32-klayout_scrot_runtime.txt
│   │   │       │   │   ├── 33-klayout.xor.log
│   │   │       │   │   ├── 34-klayout.scrot.log
│   │   │       │   │   ├── 34-klayout_scrot_runtime.txt
│   │   │       │   │   ├── 35-klayout.xor.log
│   │   │       │   │   ├── 35-klayout_xor_runtime.txt
│   │   │       │   │   ├── 39-klayout.magic.drc.log
│   │   │       │   │   ├── 39-klayout_magic_drc_runtime.txt
│   │   │       │   │   ├── 6-klayout.scrot.log
│   │   │       │   │   └── 6-klayout_scrot_runtime.txt
│   │   │       │   ├── lvs
│   │   │       │   │   ├── 24-write_powered_verilog.log
│   │   │       │   │   ├── 37-lvs.lef.log
│   │   │       │   │   └── 37-lvs_runtime.txt
│   │   │       │   ├── magic
│   │   │       │   │   ├── 26-magic.log
│   │   │       │   │   ├── 28-magic.mag.gds_ptrs.log
│   │   │       │   │   ├── 29-magic.lef.log
│   │   │       │   │   ├── 30-magic_gen_runtime.txt
│   │   │       │   │   ├── 30-magic.maglef.log
│   │   │       │   │   ├── 36-magic_ext2spice.feedback.txt
│   │   │       │   │   ├── 36-magic_ext_spice_runtime.txt
│   │   │       │   │   ├── 36-magic_spice.log
│   │   │       │   │   ├── 38-magic.drc.log
│   │   │       │   │   └── 38-magic_drc_runtime.txt
│   │   │       │   ├── obs.log
│   │   │       │   ├── placement
│   │   │       │   │   ├── 11-openphysyn_runtime.txt
│   │   │       │   │   ├── 12-opendp.log
│   │   │       │   │   ├── 12-opendp_runtime.txt
│   │   │       │   │   ├── 8-replace.log
│   │   │       │   │   ├── 9-openphysyn.log
│   │   │       │   │   └── replace_runtime.txt
│   │   │       │   ├── routing
│   │   │       │   │   ├── 17-fastroute.log
│   │   │       │   │   ├── 17-fastroute_runtime.txt
│   │   │       │   │   ├── 18-addspacers.log
│   │   │       │   │   ├── 18-addspacers_runtime.txt
│   │   │       │   │   ├── 20-tritonRoute.log
│   │   │       │   │   ├── 20-tritonRoute_runtime.txt
│   │   │       │   │   ├── 22-spef_extraction.log
│   │   │       │   │   ├── 22-spef_extraction_runtime.txt
│   │   │       │   │   ├── 40-or_antenna.log
│   │   │       │   │   ├── 41-or_antenna_runtime.txt
│   │   │       │   │   └── fastroute.log
│   │   │       │   └── synthesis
│   │   │       │       ├── 11-opensta_post_openphysyn
│   │   │       │       ├── 11-opensta_post_openphysyn_runtime.txt
│   │   │       │       ├── 1-yosys.log
│   │   │       │       ├── 1-yosys_runtime.txt
│   │   │       │       ├── 23-opensta_spef
│   │   │       │       ├── 23-opensta_spef_runtime.txt
│   │   │       │       ├── 2-opensta
│   │   │       │       └── 2-opensta_runtime.txt
│   │   │       ├── OPENLANE_VERSION
│   │   │       ├── PDK_SOURCES
│   │   │       ├── reports
│   │   │       │   ├── cts
│   │   │       │   ├── cvc
│   │   │       │   ├── final_summary_report.csv
│   │   │       │   ├── floorplan
│   │   │       │   │   ├── 3-verilog2def.core_area.rpt
│   │   │       │   │   └── 3-verilog2def.die_area.rpt
│   │   │       │   ├── klayout
│   │   │       │   │   ├── 33-klayout.xor.rpt
│   │   │       │   │   ├── 35-klayout.xor.rpt
│   │   │       │   │   └── 39-klayout.magic.lydrc
│   │   │       │   ├── lvs
│   │   │       │   ├── magic
│   │   │       │   │   ├── 38-magic.drc
│   │   │       │   │   ├── 38-magic.drc.klayout.xml
│   │   │       │   │   ├── 38-magic.drc.rdb
│   │   │       │   │   ├── 38-magic.drc.tcl
│   │   │       │   │   └── 38-magic.tr.drc
│   │   │       │   ├── manufacturability_report.rpt
│   │   │       │   ├── placement
│   │   │       │   │   ├── 8-replace.min_max.rpt
│   │   │       │   │   ├── 8-replace.rpt
│   │   │       │   │   ├── 8-replace.timing.rpt
│   │   │       │   │   ├── 8-replace_tns.rpt
│   │   │       │   │   ├── 8-replace_wns.rpt
│   │   │       │   │   ├── 9-openphysyn_allchecks.rpt
│   │   │       │   │   ├── 9-openphysyn_tns.rpt
│   │   │       │   │   ├── 9-openphysyn_violators.rpt
│   │   │       │   │   └── 9-openphysyn_wns.rpt
│   │   │       │   ├── routed_runtime.txt
│   │   │       │   ├── routing
│   │   │       │   │   ├── 17-fastroute.min_max.rpt
│   │   │       │   │   ├── 17-fastroute.rpt
│   │   │       │   │   ├── 17-fastroute.timing.rpt
│   │   │       │   │   ├── 17-fastroute_tns.rpt
│   │   │       │   │   ├── 17-fastroute_wns.rpt
│   │   │       │   │   ├── 20-tritonRoute.drc
│   │   │       │   │   ├── 20-tritonRoute.klayout.xml
│   │   │       │   │   └── 41-antenna.rpt
│   │   │       │   ├── runtime_summary_report.rpt
│   │   │       │   ├── runtime_summary_report.rpt.parsable
│   │   │       │   ├── synthesis
│   │   │       │   │   ├── 11-opensta_post_openphysyn.min_max.rpt
│   │   │       │   │   ├── 11-opensta_post_openphysyn.rpt
│   │   │       │   │   ├── 11-opensta_post_openphysyn.timing.rpt
│   │   │       │   │   ├── 11-opensta_post_openphysyn_tns.rpt
│   │   │       │   │   ├── 11-opensta_post_openphysyn_wns.rpt
│   │   │       │   │   ├── 1-yosys_4.chk.rpt
│   │   │       │   │   ├── 1-yosys_4.stat.rpt
│   │   │       │   │   ├── 1-yosys_dff.stat
│   │   │       │   │   ├── 1-yosys_pre.stat
│   │   │       │   │   ├── 23-opensta_spef.min_max.rpt
│   │   │       │   │   ├── 23-opensta_spef.rpt
│   │   │       │   │   ├── 23-opensta_spef.timing.rpt
│   │   │       │   │   ├── 23-opensta_spef_tns.rpt
│   │   │       │   │   ├── 23-opensta_spef_wns.rpt
│   │   │       │   │   ├── 2-opensta.min_max.rpt
│   │   │       │   │   ├── 2-opensta.rpt
│   │   │       │   │   ├── 2-opensta.timing.rpt
│   │   │       │   │   ├── 2-opensta_tns.rpt
│   │   │       │   │   └── 2-opensta_wns.rpt
│   │   │       │   └── total_runtime.txt
│   │   │       ├── results
│   │   │       │   ├── cts
│   │   │       │   │   ├── gcd.cts.def
│   │   │       │   │   ├── gcd.cts.def.png
│   │   │       │   │   ├── gcd.cts.obs.def
│   │   │       │   │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │       │   ├── cvc
│   │   │       │   │   ├── cvc_gcd.debug.gz
│   │   │       │   │   ├── cvc_gcd.error.gz
│   │   │       │   │   ├── cvc_gcd.log
│   │   │       │   │   ├── gcd.cdl
│   │   │       │   │   ├── gcd.power
│   │   │       │   │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │       │   ├── floorplan
│   │   │       │   │   ├── gcd.floorplan.def
│   │   │       │   │   ├── gcd.floorplan.def.png
│   │   │       │   │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │       │   ├── klayout
│   │   │       │   │   ├── gcd.gds
│   │   │       │   │   ├── gcd.gds.png
│   │   │       │   │   ├── gcd.lyp
│   │   │       │   │   ├── gcd.xor.gds
│   │   │       │   │   ├── gcd.xor.gds.png
│   │   │       │   │   ├── gcd.xor.xml
│   │   │       │   │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │       │   ├── lvs
│   │   │       │   │   ├── gcd.lvs.lef.json
│   │   │       │   │   ├── gcd.lvs.lef.log
│   │   │       │   │   ├── gcd.lvs_parsed.lef.log
│   │   │       │   │   ├── gcd.lvs.powered.v
│   │   │       │   │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │       │   ├── magic
│   │   │       │   │   ├── gcd.drc.mag
│   │   │       │   │   ├── gcd.gds
│   │   │       │   │   ├── gcd.gds.lydrc
│   │   │       │   │   ├── gcd.gds.png
│   │   │       │   │   ├── gcd.lef
│   │   │       │   │   ├── gcd.lef.mag
│   │   │       │   │   ├── gcd.lef.spice
│   │   │       │   │   ├── gcd.mag
│   │   │       │   │   ├── gcd.spice
│   │   │       │   │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │       │   ├── placement
│   │   │       │   │   ├── gcd.placement.def
│   │   │       │   │   ├── gcd.placement.def.png
│   │   │       │   │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │       │   ├── routing
│   │   │       │   │   ├── gcd.def
│   │   │       │   │   ├── gcd.def.png
│   │   │       │   │   ├── gcd.def.ref
│   │   │       │   │   ├── gcd.spef
│   │   │       │   │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │       │   └── synthesis
│   │   │       │       ├── gcd.synthesis_cts.v
│   │   │       │       ├── gcd.synthesis_optimized.v
│   │   │       │       ├── gcd.synthesis_preroute.v
│   │   │       │       ├── gcd.synthesis.v
│   │   │       │       └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │       └── tmp
│   │   │           ├── cts
│   │   │           │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │           ├── cvc
│   │   │           │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │           ├── floorplan
│   │   │           │   ├── 3-verilog2def_openroad.def
│   │   │           │   ├── 4-ioPlacer.def
│   │   │           │   ├── 7-pdn.def
│   │   │           │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │           ├── klayout
│   │   │           │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │           ├── lvs
│   │   │           │   ├── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │           │   └── setup_file.lef.lvs
│   │   │           ├── magic
│   │   │           │   ├── gcd.ext
│   │   │           │   ├── magic_gds_ptrs.mag
│   │   │           │   ├── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │           │   ├── sky130_fd_sc_hd__a2111oi_2.ext
│   │   │           │   ├── sky130_fd_sc_hd__a21bo_2.ext
│   │   │           │   ├── sky130_fd_sc_hd__a21boi_0.ext
│   │   │           │   ├── sky130_fd_sc_hd__a21oi_2.ext
│   │   │           │   ├── sky130_fd_sc_hd__a221o_2.ext
│   │   │           │   ├── sky130_fd_sc_hd__a22o_2.ext
│   │   │           │   ├── sky130_fd_sc_hd__a2bb2oi_2.ext
│   │   │           │   ├── sky130_fd_sc_hd__a31o_2.ext
│   │   │           │   ├── sky130_fd_sc_hd__a32o_2.ext
│   │   │           │   ├── sky130_fd_sc_hd__a41o_2.ext
│   │   │           │   ├── sky130_fd_sc_hd__and3_2.ext
│   │   │           │   ├── sky130_fd_sc_hd__buf_1.ext
│   │   │           │   ├── sky130_fd_sc_hd__clkbuf_16.ext
│   │   │           │   ├── sky130_fd_sc_hd__clkbuf_1.ext
│   │   │           │   ├── sky130_fd_sc_hd__decap_12.ext
│   │   │           │   ├── sky130_fd_sc_hd__decap_3.ext
│   │   │           │   ├── sky130_fd_sc_hd__decap_4.ext
│   │   │           │   ├── sky130_fd_sc_hd__decap_6.ext
│   │   │           │   ├── sky130_fd_sc_hd__decap_8.ext
│   │   │           │   ├── sky130_fd_sc_hd__dfxtp_2.ext
│   │   │           │   ├── sky130_fd_sc_hd__fill_1.ext
│   │   │           │   ├── sky130_fd_sc_hd__fill_2.ext
│   │   │           │   ├── sky130_fd_sc_hd__inv_2.ext
│   │   │           │   ├── sky130_fd_sc_hd__lpflow_clkbufkapwr_1.ext
│   │   │           │   ├── sky130_fd_sc_hd__lpflow_clkinvkapwr_1.ext
│   │   │           │   ├── sky130_fd_sc_hd__lpflow_clkinvkapwr_2.ext
│   │   │           │   ├── sky130_fd_sc_hd__lpflow_inputiso0n_1.ext
│   │   │           │   ├── sky130_fd_sc_hd__lpflow_isobufsrc_1.ext
│   │   │           │   ├── sky130_fd_sc_hd__nand2_2.ext
│   │   │           │   ├── sky130_fd_sc_hd__nor2_2.ext
│   │   │           │   ├── sky130_fd_sc_hd__o211a_2.ext
│   │   │           │   ├── sky130_fd_sc_hd__o21ai_0.ext
│   │   │           │   ├── sky130_fd_sc_hd__o221a_2.ext
│   │   │           │   ├── sky130_fd_sc_hd__o22a_2.ext
│   │   │           │   ├── sky130_fd_sc_hd__o2bb2a_2.ext
│   │   │           │   ├── sky130_fd_sc_hd__o311ai_0.ext
│   │   │           │   ├── sky130_fd_sc_hd__o311ai_2.ext
│   │   │           │   ├── sky130_fd_sc_hd__or4_2.ext
│   │   │           │   ├── sky130_fd_sc_hd__or4b_2.ext
│   │   │           │   ├── sky130_fd_sc_hd__tapvpwrvgnd_1.ext
│   │   │           │   └── sky130_fd_sc_hd__xnor3_1.ext
│   │   │           ├── magic_spice.tcl
│   │   │           ├── merged.lef
│   │   │           ├── merged_unpadded.lef
│   │   │           ├── met_layers_list.txt
│   │   │           ├── opt.lib
│   │   │           ├── placement
│   │   │           │   ├── 8-replace.def
│   │   │           │   ├── 9-openphysyn.def
│   │   │           │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │           ├── routing
│   │   │           │   ├── 17-fastroute.def
│   │   │           │   ├── 17-fastroute.guide
│   │   │           │   ├── 18-addspacers.def
│   │   │           │   ├── 20-tritonRoute.guide
│   │   │           │   ├── 20-tritonRoute.param
│   │   │           │   ├── 20-tritonRoute_TA.def
│   │   │           │   ├── 24-gcd.powered.def
│   │   │           │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │           ├── sky130_fd_sc_hd__tt_025C_1v80.no_pg.lib
│   │   │           ├── synthesis
│   │   │           │   ├── hierarchy.dot
│   │   │           │   ├── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │           │   └── yosys.sdc
│   │   │           ├── tracks_copy.info
│   │   │           └── trimmed.lib
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── gcd.v
│   │       └── README.md
│   ├── get_docker_config.py
│   ├── Makefile
│   ├── patches
│   │   ├── Add-directory-support-bashrc.diff
│   │   └── Add-directory-support-zshrc.diff
│   └── README.md
├── signoff
│   └── gcd
│       ├── final_summary_report.csv
│       ├── OPENLANE_VERSION
│       └── PDK_SOURCES
├── spi
│   └── lvs
│       └── gcd.spice
└── verilog
    └── gl
        └── gcd.v

58 directories, 290 files

