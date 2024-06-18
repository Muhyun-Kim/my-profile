<script lang="ts">
</script>

<div class="contact-page">
	<div class="contact-page-frame">
		<h1>Contact</h1>
		<div class="contact">
			<div class="contact-info">
				<p>連絡をお待ちしております。</p>
				<div>
					<h3>Email</h3>
					<p>muhyun.kim.dev@gmail.com</p>
				</div>
			</div>
			<form action="submit" class="contact-form">
				<div class="form-frame">
					<div class="form-l">
						<div class="submit-el">
							<label for="email">メールアドレス</label>
							<input id="email" name="email" type="email" />
						</div>
						<div class="submit-el">
							<label for="email">お名前</label>
							<input id="name" name="name" type="text" />
						</div>
						<div class="submit-el">
							<label for="email">件名</label>
							<input id="tilte" name="title" type="text" />
						</div>
					</div>
					<div class="form-r">
						<div class="submit-el">
							<label for="email">本文</label>
							<textarea id="body" name="body"></textarea>
						</div>
					</div>
				</div>
				<button>Contact</button>
			</form>
		</div>
	</div>
</div>

<style>
	.contact-page {
		display: flex;
		justify-content: center;
	}
	.contact-page-frame {
		width: 80%;
	}
	.contact {
		display: flex;
		justify-content: space-between;
		width: 100%;
	}
	.contact-info,
	.contact-form {
		width: 50%;
	}
	.contact-info {
		display: flex;
		flex-direction: column;
		justify-content: space-between;
	}
	.contact-form {
		display: flex;
		flex-direction: column;
	}
	.form-frame {
		display: flex;
		justify-content: space-between;
		width: 100%;
	}
	.form-l,
	.form-r {
		width: 45%;
	}
	.submit-el {
		display: flex;
		flex-direction: column;
		padding-bottom: 16px;
	}
	.form-r .submit-el {
		display: flex;
		height: 100%;
	}
	.submit-el textarea {
		height: fit-content;
		flex-grow: 1;
	}
	.submit-el label {
		margin-bottom: 8px;
	}
	input,
	textarea {
		border: 1px solid #000;
		border-radius: 5px;
	}
</style>
