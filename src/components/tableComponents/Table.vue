<template>
  <div>
    <table class="table zebra">
      <thead>
        <TableRow>
          <TableHeader>Nome</TableHeader>
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
          
          <TableCell :tamanho="80">
            <Button tipo="acao" texto="" acao="editar" icone="fa-pen" />
            <Button tipo="acao" texto="" acao="apagar" icone="fa-trash" />
          </TableCell>
        </TableRow>
      </tbody>
    </table>
  </div>
</template>

<script>
import TableHeader from "../tableComponents/TableHeader";
import TableRow from "../tableComponents/TableRow";
import TableCell from "../tableComponents/TableCell";
import Button from "./../form/Button";
export default {
  name: "Table",
  components: { TableHeader, TableRow, TableCell, Button },
};
</script>

<style>


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