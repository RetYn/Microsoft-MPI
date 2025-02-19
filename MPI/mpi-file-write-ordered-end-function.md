---
title: MPI_File_write_ordered_end function
TOCTitle: MPI_File_write_ordered_end function
ms:assetid: 6c913bcb-7af0-4ffe-bbb6-321de5bb7be5
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Dn473370(v=VS.85)
ms:contentKeyID: 59360906
ms.date: 03/28/2018
mtps_version: v=VS.85
f1_keywords:
- MPI_FILE_WRITE_ORDERED_END
- mpif/MPI_File_write_ordered_end
- mpi/MPI_FILE_WRITE_ORDERED_END
dev_langs:
- C++
- C
description: "Learn Microsoft MPI File Write Ordered End Function: Complete split collective writes with shared file pointers. Boost your HPC Pack skills today."
---

# MPI\_File\_write\_ordered\_end function

Completes a split collective write using shared file pointer.

## Syntax

``` c++
int MPIAPI MPI_File_write_ordered_end(
        MPI_File   file,
  _In_  void       *buf,
  _Out_ MPI_Status *status
);
```

## Parameters

  - *file*  
    File handle.

  - *buf* \[in\]  
    Initial address of buffer.

  - *status* \[out\]  
    Status object.

## Return value

Returns **MPI\_SUCCESS** on success. Otherwise, the return value is an error code.

In Fortran, the return value is stored in the *IERROR* parameter.

## Fortran

``` FORTRAN
    MPI_FILE_WRITE_ORDERED_END(FH, BUF, STATUS, IERROR)
        <type> BUF(*)
        INTEGER FH, STATUS(MPI_STATUS_SIZE), IERROR
```

## Requirements

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Product</p></td>
<td><p>HPC Pack 2012 MS-MPI Redistributable Package, HPC Pack 2008 R2 MS-MPI Redistributable Package, HPC Pack 2008 MS-MPI Redistributable Package or HPC Pack 2008 Client Utilities</p></td>
</tr>
<tr class="even">
<td><p>Header</p></td>
<td>Mpi.h;
Mpif.h</td>
</tr>
<tr class="odd">
<td><p>Library</p></td>
<td>Msmpi.lib</td>
</tr>
<tr class="even">
<td><p>DLL</p></td>
<td>Msmpi.dll</td>
</tr>
</tbody>
</table>


## See also

[MPI File Functions](mpi-file-functions.md)

