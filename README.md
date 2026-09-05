# HVAC Nameplate / Fault-Code Workflow (Educational)

Python **stdlib-only** CLI to capture nameplate fields and look up a small starter set of educational fault-code stubs (generic + a few major brands).

> **Incomplete database — verify with OEM manuals.**  
> Service Tech chat can use photos for nameplate transcription.

## Quick start

```bash
cd hvac-nameplate-fault-codes
python3 nameplate_faults.py --help
python3 nameplate_faults.py --list-codes
python3 nameplate_faults.py -i
```

### Example

```bash
python3 nameplate_faults.py \
  --brand carrier --model 24ACC636 \
  --serial 1234 --voltage 230 \
  --refrigerant R-410A --charge 8.5 \
  --code 41 --save
```

Cards can be appended to a local JSON store (`~/.hvac_nameplate_faults.json` by default).
