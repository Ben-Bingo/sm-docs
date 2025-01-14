---
sidebar_position: 25
title: Storage
hide_title: true
sidebar-label: 'Storage'
---

<br></br>

## Storage

**Associated namespace:** [sm.storage](/docs/Game-Script-Environment/Static-Functions/sm.storage)

A userdata object representing a <strong>storage</strong> object.

:::info note
The storage object is only accessible via <code>self.storage</code> in scripted objects (see [classes](/docs/Game-Script-Environment/Classes/CommonCallbacks)).

The storage object also allows for data to be saved in creations saved on the Lift.
:::

## Functions

### load

```lua
storage:load()
```
<code>Server-Only</code> <br></br>

Returns the data stored in the storage object. <br></br>
Returns nil if the object contains no data.

<strong>Arguments:</strong> <br></br>

- <code>storage</code> [<strong> <a href="/docs/Game-Script-Environment/Userdata/Storage"> Storage </a> </strong>]: The storage.

<strong>Returns:</strong> <br></br>

- [<strong> any </strong>]: The data.

---

### save

```lua
storage:save( data )
```
<code>Server-Only</code> <br></br>

Saves any Lua data into the storage object.

The data will remain stored after closing the world, and is retrieved using [load](#load).

<strong>Arguments:</strong> <br></br>

- <code>storage</code> [<strong> <a href="/docs/Game-Script-Environment/Userdata/Storage"> Storage </a> </strong>]: The storage.
- <code>data</code> [<strong> any </strong>]: The data.

---