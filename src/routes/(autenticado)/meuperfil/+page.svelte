<script>
	let { data, form } = $props();

	console.log(data);
</script>

<div class="mx-auto card my-3" style="max-width: 540px;">
	<div class="row g-0">
		<div class="col-md-4 text-center">
			<img src={data.user.image ?? '/person.svg'} class="img-fluid rounded-start" alt="foto do usuário" />
		</div>
		<div class="col-md-8">
			<div class="card-body">
				<form class="row g-3">
					<div class="col-md-6">
						<label for="nomeUsuario" class="form-label">Nome do usuário</label>
						<input class="form-control" id="nomeUsuario" value={data.user.username} />
					</div>
					<div class="col-md-6">
						<label for="senha" class="form-label">Senha atual</label>
						<input type="password" class="form-control" id="senha" />
					</div>
					<div class="col-md-6">
						<label for="senha1" class="form-label">Nova senha</label>
						<input type="password" class="form-control" id="senha1" />
					</div>
					<div class="col-md-6">
						<label for="senha2" class="form-label">Confirme a senha</label>
						<input type="password" class="form-control" id="senha2" />
					</div>
					<div class="col-12">
						<label for="fotoPerfil" class="form-label">Foto de perfil</label>
						<input class="form-control" type="file" id="fotoPerfil" />
					</div>
					<div class="col-12">
						<button class="btn btn-primary">Atualizar informações</button>
					</div>
				</form>
			</div>
		</div>
	</div>
</div>
