<template>
  <div>
    <table class="table zebra">
      <thead>
        <TableRow>
          <TableHeader>Nome"</TableHeader>
          <TableHeader>Sobrenome</TableHeader>
          <TableHeader>Email</TableHeader>
          <TableHeader>Bitcoin</TableHeader>
          <TableHeader></TableHeader>
        </TableRow>
      </thead>
      <tbody>
        <TableRow>
          <TableCell>1</TableCell>
          <TableCell>1</TableCell>
          <TableCell>1</TableCell>
          <TableCell>1</TableCell>
          <TableCell>
            <Button tipo="acao" texto="" acao="editar" icone="fa-pen" />
            <Button tipo="acao" texto="" acao="apagar" icone="fa-trash" />
          </TableCell>
        </TableRow>
        <TableRow>
          <TableCell>1</TableCell>
          <TableCell>1</TableCell>
          <TableCell>1</TableCell>
          <TableCell>1</TableCell>
          <TableCell>1</TableCell>
        </TableRow>
      </tbody>
    </table>
  </div>
</template>

<script>
import TableHeader from "../tableComponents/TableHeader";
import TableRow from "../tableComponents/TableRow";
import TableCell from "../tableComponents/TableCell";
import Button from "./Button";
export default {
  name: "Table",
  components: { TableHeader, TableRow, TableCell, Button },
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

tbody tr {
  border-left: #fff 2px solid;
}

.zebra tbody tr:hover {
  background: #fff;
  border-left: #007bff 2px solid;
}
</style>