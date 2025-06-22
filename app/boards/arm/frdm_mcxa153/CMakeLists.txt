#
# Copyright 2025 NXP
#
# SPDX-License-Identifier: Apache-2.0
#

zephyr_library()
zephyr_library_sources(board.c)

board_set_flasher_ifnset(none)

set(BOARD_MCUX true)

zephyr_include_directories(${ZEPHYR_BASE}/soc/arm/nxp_mcx)
