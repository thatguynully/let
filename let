#!/usr/bin/env bash
# SPDX-License-Identifier: GPL-3.0-or-later

set -e

usage() {
  echo "Usage: let <package> in|out" >&2
  exit 1
}

if [ "$#" -ne 2 ]; then
  usage
fi

package="$1"
action="$2"

case "$action" in
  in)
    sudo pacman -S --needed "$package"
    ;;
  out)
    sudo pacman -Rns "$package"
    ;;
  *)
    usage
    ;;
esac
