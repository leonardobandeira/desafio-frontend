<template>
  <div>
    <table class="table zebra">
      <thead>
        <TableRow>
          <TableHeader texto="Nome" />
          <TableHeader texto="Sobrenome" />
          <TableHeader texto="Email" />
          <TableHeader texto="Bitcoin" />
          <TableHeader texto="" />
        </TableRow>
      </thead>
      <tbody>
        <TableRow>
          <TableCell texto="1" />
          <TableCell texto="João" />
          <TableCell texto="30" />
        </TableRow>
        <TableRow>
          <TableCell texto="2" />
          <TableCell texto="Maria" />
          <TableCell texto="25" />
        </TableRow>
      </tbody>
    </table>
  </div>
</template>

<script>
import TableHeader from "../tableComponents/TableHeader";
import TableRow from "../tableComponents/TableRow";
import TableCell from "../tableComponents/TableCell";
export default {
  name: "Table",
  components: { TableHeader, TableRow, TableCell },
};
</script>

<style>
.content__tabela {
  background: #fff;
  box-shadow: 0px 5px 5px rgba(0, 0, 0, 0.1);
  border-radius: 4px;
  justify-content: left;
  padding: 1.5em 0.5em;
}

.table-container {
  margin: 0 auto;
}

.table {
  width: 100%;
  border-collapse: collapse;
}

.table th,
.table td {
  padding: 8px;
  text-align: left;
}

.zebra tbody tr:nth-child(odd) {
  background-color: #f2f2f2;
}

tbody tr{
  border-left: #fff 2px solid;
}

tbody tr:hover{
  background: #fff;
  border-left: #007bff 2px solid;
}
</style>