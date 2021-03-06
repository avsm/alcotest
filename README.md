## Alcotest

Alcotest is a lightweight and colourful test framework, based on OUnit.

Alcotest exposes a much more restricted interface than OUnit, as you can
only pass to `Alcotest.run` a tree of callbacks of depth 2, and the
callbacks are `unit -> unit` functions that you can build using the
usual `OUnit.assert_*` functions or any other means (including
Quickcheck-like test generators).

This limitation enables Alcotest to provide a quiet and colorful
output where only faulty runs are fully displayed at the end of the
run (with the full logs ready to inspect), with a simple (yet
expressive) query language to select the tests to run.
