.PHONY: make_keymap_keebio_iris_rev6 copy_keymap_keebio_iris_rev6 compile_firmware_keebio_iris_rev6 run_iris_rev6 make_keymap setup_qmk copy_keymap compile_firmware copy_firmware clean

clean:
	cd .. && rm -rf .build
	cd .. *.hex

make_keymap_keebio_iris_rev6:
	cd .. && qmk json2c personal/keebio_iris_rev6/keymap.json -o personal/keebio_iris_rev6/keymap.c
	rm keebio_iris_rev6/keymap.c.bak

copy_keymap_keebio_iris_rev6:
	cd .. && cp -r personal/keebio_iris_rev6/* keyboards/keebio/iris/keymaps/personal

compile_firmware_keebio_iris_rev6:
	cd .. && qmk compile -kb keebio/iris/rev6 -km personal

flash_firmware_keebio_iris_rev6:
	cd .. && qmk flash -kb keebio/iris/rev6 -km personal

run_iris_rev6: clean make_keymap_keebio_iris_rev6 copy_keymap_keebio_iris_rev6 compile_firmware_keebio_iris_rev6

flash_iris_rev6: clean make_keymap_keebio_iris_rev6 copy_keymap_keebio_iris_rev6 flash_firmware_keebio_iris_rev6

make_keymap_keebio_iris_rev7:
	cd .. && qmk json2c personal/keebio_iris_rev7/keymap.json -o personal/keebio_iris_rev7/keymap.c
	rm keebio_iris_rev7/keymap.c.bak

copy_keymap_keebio_iris_rev7:
	cd .. && cp -r personal/keebio_iris_rev7/* keyboards/keebio/iris/keymaps/personal

compile_firmware_keebio_iris_rev7:
	cd .. && qmk compile -kb keebio/iris/rev7 -km personal

flash_firmware_keebio_iris_rev7:
	cd .. && qmk flash -kb keebio/iris/rev7 -km personal

run_iris_rev7: clean make_keymap_keebio_iris_rev7 copy_keymap_keebio_iris_rev7 compile_firmware_keebio_iris_rev7

flash_iris_rev7: clean make_keymap_keebio_iris_rev7 copy_keymap_keebio_iris_rev7 flash_firmware_keebio_iris_rev7

flash_pageturner:
	cd .. && qmk flash -kb pageturner -km default

make_keymap_piantor_pro:
	cd .. && qmk json2c personal/piantor_pro/keymap.json -o personal/piantor_pro/keymap.c
	rm piantor_pro/keymap.c.bak

copy_keymap_piantor_pro:
	cd .. && cp -r personal/piantor_pro/* keyboards/beekeeb/piantor_pro/keymaps/personal

compile_firmware_piantor_pro:
	cd .. && qmk compile -kb beekeeb/piantor_pro -km personal

flash_firmware_piantor_pro:
	cd .. && qmk flash -kb beekeeb/piantor_pro -km personal

run_piantor_pro: clean make_keymap_piantor_pro copy_keymap_piantor_pro compile_firmware_piantor_pro

flash_piantor_pro: clean make_keymap_piantor_pro copy_keymap_piantor_pro flash_firmware_piantor_pro

make_keymap_boardsource_unicorne:
	cd .. && qmk json2c personal/boardsource_unicorne/keymap.json -o personal/boardsource_unicorne/keymap.c
	rm boardsource_unicorne/keymap.c.bak

copy_keymap_boardsource_unicorne:
	cd .. && cp -r personal/boardsource_unicorne/* keyboards/boardsource/unicorne/keymaps/personal

compile_firmware_boardsource_unicorne_left:
	cd .. && qmk compile -kb boardsource/unicorne -km personal -bl uf2-split-left

compile_firmware_boardsource_unicorne_right:
	cd .. && qmk compile -kb boardsource/unicorne -km personal -bl uf2-split-right

flash_firmware_boardsource_unicorne_left:
	cd .. && qmk flash -kb boardsource/unicorne -km personal -bl uf2-split-left

flash_firmware_boardsource_unicorne_right:
	cd .. && qmk flash -kb boardsource/unicorne -km personal -bl uf2-split-right

run_boardsource_unicorne_left: clean make_keymap_boardsource_unicorne copy_keymap_boardsource_unicorne compile_firmware_boardsource_unicorne_left
run_boardsource_unicorne_right: clean make_keymap_boardsource_unicorne copy_keymap_boardsource_unicorne compile_firmware_boardsource_unicorne_right

flash_boardsource_unicorne_left: clean make_keymap_boardsource_unicorne copy_keymap_boardsource_unicorne flash_firmware_boardsource_unicorne_left
flash_boardsource_unicorne_right: clean make_keymap_boardsource_unicorne copy_keymap_boardsource_unicorne flash_firmware_boardsource_unicorne_right

make_keymap_bastardkb_tbkmini:
	cd .. && qmk json2c personal/bastardkb_tbkmini/keymap.json -o personal/bastardkb_tbkmini/keymap.c
	rm bastardkb_tbkmini/keymap.c.bak

copy_keymap_bastardkb_tbkmini:
	cd .. && cp -r personal/bastardkb_tbkmini/* keyboards/bastardkb/tbkmini/keymaps/personal

compile_firmware_bastardkb_tbkmini_left:
	cd .. && qmk compile -kb bastardkb/tbkmini/v2/splinky_3 -km personal -bl uf2-split-left

compile_firmware_bastardkb_tbkmini_right:
	cd .. && qmk compile -kb bastardkb/tbkmini/v2/splinky_3 -km personal -bl uf2-split-right

flash_firmware_bastardkb_tbkmini_left:
	cd .. && qmk flash -kb bastardkb/tbkmini/v2/splinky_3 -km personal -bl uf2-split-left

flash_firmware_bastardkb_tbkmini_right:
	cd .. && qmk flash -kb bastardkb/tbkmini/v2/splinky_3 -km personal -bl uf2-split-right

run_bastardkb_tbkmini_left: clean make_keymap_bastardkb_tbkmini copy_keymap_bastardkb_tbkmini compile_firmware_bastardkb_tbkmini_left
run_bastardkb_tbkmini_right: clean make_keymap_bastardkb_tbkmini copy_keymap_bastardkb_tbkmini compile_firmware_bastardkb_tbkmini_right

flash_bastardkb_tbkmini_left: clean make_keymap_bastardkb_tbkmini copy_keymap_bastardkb_tbkmini flash_firmware_bastardkb_tbkmini_left
flash_bastardkb_tbkmini_right: clean make_keymap_bastardkb_tbkmini copy_keymap_bastardkb_tbkmini flash_firmware_bastardkb_tbkmini_right
